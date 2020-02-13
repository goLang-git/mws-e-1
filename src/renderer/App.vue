<template>
  <div id="app">
    <titles/>

    <router-view></router-view>
  </div>
</template>

<script>
import titles from './components/window_title/title'

  export default {
    name: 'app',
    components:{
      titles

    }
  }
</script>

<style>
  html,body{
    margin:0;
    padding:0;
    min-width:300px;
  }
</style>
