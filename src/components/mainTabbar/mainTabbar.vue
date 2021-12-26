<template>
  <div>
    <tabbar>
      <tab-bar-item path="/home">
        <i slot="item-icon" class="el-icon-s-home"></i>
        <i slot="item-icon-active" class="el-icon-s-home" style="color: red"></i>
        <div slot="item-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/category">
        <i slot="item-icon" class="el-icon-menu"></i>
        <i slot="item-icon-active" class="el-icon-menu" style="color: red"></i>
        <div slot="item-text">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/cart">
        <i slot="item-icon" class="el-icon-shopping-cart-2"></i>
        <i slot="item-icon-active" class="el-icon-shopping-cart-2" style="color: red"></i>
        <div slot="item-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <i slot="item-icon" class="el-icon-user"></i>
        <i slot="item-icon-active" class="el-icon-user" style="color: red"></i>
        <div slot="item-text">我的</div>
      </tab-bar-item>
    </tabbar>
  </div>
</template>

<script>
import tabbar from '../tabbar/tabbar.vue'
import TabBarItem from '../tabbarItem/TabBarItem.vue'
export default {
  components: {
    tabbar,
    TabBarItem
  }
}
</script>

<style>

</style>