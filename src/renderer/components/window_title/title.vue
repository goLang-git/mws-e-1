<template>
    <div class="headers" style="-webkit-app-region: drag">

            <div  class="gb" style="-webkit-app-region: no-drag">
                <span class="iconfont icon-close-line"style="font-size:17px;-webkit-app-region: no-drag"></span>
            </div>

                <div  class="sx" style="-webkit-app-region: no-drag">
                    <span class="iconfont icon-xiaoxitixingchuangkoudanchufangshi"style="font-size:17px;"></span>
                </div>
            <div class="fx" style="-webkit-app-region: no-drag">
                <span class="iconfont icon-suoxiao" style="font-size:17px;"></span>
            </div>
            <tab/>
    </div>
</template>
<script>
    import tab  from '../Tab_Bar/tabbar'
export default {
    name:'title',
    components:{
        tab
    }

}
</script>
<style scoped>
    .headers{
        width:100%;
        height:30px;
        background-color:#f1f1f2;

    }





    
    
    

   


    div{
        float: right;
        width:50px;
        color:#000000;
        text-align:center;
        margin-right: 0;
        height:30px;
        line-height: 30px;
        font-weight:900;
    }
    .fx:hover,.sx:hover{
        
        background:rgba(0,0,0,.1);
        color:#000000;
        
    }
    .gb:hover{
          background:#ae1906;
        color:#FFFFFF;
    }
    div:after{
        content:'';
        display: block;
        clear:both;
    }
  
</style>