<template>
    <div @click="denglu">
        我是登录页面
    </div>
</template>
<script>
export default {
    methods:{
        denglu(){
            this.$router.push('/indexs')
        }
    }
}
</script>
<style scoped>

</style>