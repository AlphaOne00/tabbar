<template>
  <div class="tab-bar-item" @click="itemClick">
    <div v-if="!isActive" ><slot name="item-icon"></slot></div>
    <div v-else><slot name="item-icon-active"></slot></div>
    <div :style="activeStyle">
      <slot name="item-text" ></slot> 
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
    }
  },
  props: {
    path:String,
    activeColor:{
      type: String,
      default: 'red'
    }
  },
  computed: {
    isActive() {
      /* this.$route是当前活跃的路由
         indexOf() 判断是否包含
         === -1 表示找到了 */
      return this.$route.path.indexOf(this.path) !== -1
    },
    activeStyle() {
      return this.isActive ? {color: this.activeColor} : {}
    }
  },
  methods: {
    itemClick() {
      this.$router.replace(this.path)
    }
  }
}
</script>

<style>
.tab-bar-item {
  flex: 1;
  text-align: center;
  height: 49px;
}
i{
  font-size: 24px;
}

</style>