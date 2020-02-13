<template>
    <div class="nav">
        <div class="centers">
            <el-header>
                <el-menu   :router="true" mode="horizontal">
                    <el-menu-item index="1">{{$route.path}}</el-menu-item>
                    <el-menu-item index="/xuanping">报告</el-menu-item>
                    <el-menu-item index="3">产品</el-menu-item>
                    <el-menu-item index="4">订单</el-menu-item>
                    <el-menu-item index="5">仓库</el-menu-item>
                </el-menu>
            </el-header>
        </div>
        <div class="rights"></div>
    </div>
</template>

<script>
    export default {
        name: "One_Nav",
        data() {
            return {
                activeIndex: '1',
                activeIndex2: '1'
            };
        }
    }
</script>

<style scoped>
    .nav{
        width:100%;
        height:50px;
        display:flex;


    }

    .centers{
        flex-grow: 9;
        background: red;
    }
    .rights{
        flex-grow: 1;
        background: indigo;
    }
    .el-header{
        width:100%;
        height:50px !important;
        background: aqua;
        padding:unset;
    }
    .el-menu-item{
        line-height: 50px !important;
        height:50px !important;
    }

</style>