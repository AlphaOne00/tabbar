<template>
  <div id="app">
    <router-view />
    <mian-tabbar />
  </div>
</template>

<script>
import mianTabbar from './components/mainTabbar/mainTabbar.vue'
export default {
  components:{
    mianTabbar
  }
}
</script>
<style>
@import "./assets/css/base.css";
</style>
