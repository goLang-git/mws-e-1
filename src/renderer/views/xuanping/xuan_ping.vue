<template>
   <div class="content">
       <el-container style="height:100%;">
           <el-aside width="200px">
               <el-menu :default-openeds="['1', '3']"router="true" mode="vertical"  :select="dakai()">
                   <el-submenu index="1">
                       <template slot="title"><i class="el-icon-menu"></i><i style="color:red;">京东</i></template>
                   </el-submenu>

                   <el-submenu index="2">
                       <template slot="title"><i class="el-icon-menu"></i>京东</template>
                           <el-menu-item index="2-1">京东网</el-menu-item>
                   </el-submenu>
                   <el-submenu index="3">
                       <template slot="title"><i class="el-icon-setting"></i>拼多多</template>
                           <el-menu-item index="3-1">选项1</el-menu-item>
                   </el-submenu>

               </el-menu>
           </el-aside>

           <el-container>
               <router-view></router-view>
           </el-container>
       </el-container>


   </div>
</template>
<!---->
<script>
    export default {
        name: "xuan_ping",
        methods:{
            dakai(){
                console.log("打开")
            }
        }
    }
</script>

<style scoped>
.content {
    width: 100%;
    padding-top:80px !important;
    height:calc(100vh - 80px);

}
.el-submenu{
    background-color: #FFFFFF !important;
    color:#FFFFFF !important;
}
.el-header {
    background-color: #B3C0D1;
    color: #333;
    line-height: 60px;
}
.el-submenu__title{
    color:red !important;
}
.el-aside {

    overflow-x: hidden!important;
    overflow-y: auto !important;
    background-color:#EDEDED;
    height:100%;
    color:wheat!important;
    border-right: 1px solid #e6e6e6;
}
    /*.el-main{*/
    /*    height:100%;*/
    /*    overflow: auto;*/

    /*}*/
    .el-menu-item{
        background:#FFFFFF !important;

    }
    .el-menu{
        background-color: #EDEDED !important;

    border:unset;
    }

</style>