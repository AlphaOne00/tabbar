<template>
  <div>
      <div id="tabbar">
      <!-- <div class="tab-bar-item">首页</div>
      <div class="tab-bar-item">关于</div>
      <div class="tab-bar-item">购物车</div>
      <div class="tab-bar-item">我的</div> -->
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
#tabbar {
  display: flex;
  background-color: #f6f6f6;

  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
}

</style>