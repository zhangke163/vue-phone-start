<template>
<div>
<mt-header title="信息管理系统"></mt-header>
<!-- 路由留坑 -->
<router-view />
  <mt-tabbar v-model="selected">
    <mt-tab-item id="home">
      <img slot="icon" src="./assets/img/sy.png">
      首页
    </mt-tab-item>
    <mt-tab-item id="member">
      <img slot="icon" src="./assets/img/st.png">
      会员
    </mt-tab-item>
    <mt-tab-item id="shopcart">
      <img slot="icon" src="./assets/img/gw.png">
      购物车
    </mt-tab-item>
    <mt-tab-item id="search">
      <img slot="icon" src="./assets/img/ss.png">
      查找
    </mt-tab-item>
</mt-tabbar>
</div>
</template>
<script>
export default {
  data () {
    return {
      selected: ''
    }
  },
  watch: {
    selected (newV, oldV) {
      this.$router.push({
        name: newV
      })
    }
  }
}
</script>
<style>
body{
  margin:0
}
</style>
