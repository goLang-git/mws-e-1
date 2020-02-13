<template>
    <div class="baba">
        <el-main>
            <webview id="foo" src="https://www.1688.com/" allowpopups></webview>
        </el-main>

    </div>
</template>
<!-- const webview = document.getElementById('foo')
webview.addEventListener('new-window', (e) => {
    const protocol = require('url').parse(e.url).protocol;
    if (protocol === 'http:' || protocol === 'https:') {
        webview.src = e.url;
    }
});
————————————————
版权声明：本文为CSDN博主「MrGao丶」的原创文章，遵循 CC 4.0 BY-SA 版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/chenzhigaoa/article/details/80284653-->
<script>
    export default {
        name: "baba"
    }
</script>

<style scoped>

    .baba {
        width: 100%;
        height:calc(100vh - 80px);
        background:#FFFFFF;

    }
    .el-main{
        height:100%;
        overflow:auto;
        padding:unset;

    }
    webview{
        width:100%;
        height:100% !important;
    }
</style>