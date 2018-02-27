<template>
<van-tabbar v-model="active">
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

</style>
