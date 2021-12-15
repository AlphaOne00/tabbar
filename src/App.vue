<template>
  <div id="app">
    <router-view />
    <tabbar>
      <tab-bar-item path="/home">
        <div slot="item-text">首页</div>
        <i slot="item-icon" class="el-icon-s-home"></i> 
      </tab-bar-item>
      <tab-bar-item path="/category">
        <div slot="item-text">分类</div>
        <i slot="item-icon" class="el-icon-menu"></i> 
      </tab-bar-item>
      <tab-bar-item path="/cart">
        <div slot="item-text">购物车</div>
        <i slot="item-icon" class="el-icon-shopping-cart-2"></i> 
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <div slot="item-text">我的</div>
        <i slot="item-icon" class="el-icon-user"></i> 
      </tab-bar-item>
    </tabbar>
  </div>
</template>

<script>
import tabbar from './components/tabbar/tabbar.vue'
import TabBarItem from './components/tabbarItem/TabBarItem.vue'
export default {
  components:{
    tabbar,
    TabBarItem
  }
}
</script>
<style>
@import "./assets/css/base.css";
</style>
