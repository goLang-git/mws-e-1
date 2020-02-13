<template>
   <div class="content">
    <el-container>
        <el-header>Header</el-header>
        <el-aside width="300px"style="background: red;">Aside</el-aside>
        <el-main>main</el-main>
    </el-container>
   </div>
</template>
<!---->
<script>
    export default {
        name: "xuan_ping"
    }
</script>

<style scoped>
.content{
    position: fixed;
    top:80px;
}
</style>