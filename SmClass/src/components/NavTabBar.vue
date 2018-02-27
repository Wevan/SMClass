<template>
<van-tabbar v-model="active" class="nav">
  <van-tabbar-item icon="wap-home">主页</van-tabbar-item>
  <van-tabbar-item icon="chat" dot>社交</van-tabbar-item>
  <van-tabbar-item icon="records" info="5">个人</van-tabbar-item>
</van-tabbar>
</template>

<script>
export default {
  name: "nav-tab-bar",
  data() {
    return {
      active: 0
    };
  }
};
</script>

<style scoped>
.nav {
    /* width:100%; */
    /* height:30px; */
    /* margin:0 auto; */
    position:fixed;
    bottom:0;
    /* text-align:center; */
}
</style>
