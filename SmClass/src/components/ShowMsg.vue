<template>

  <div class="mx">
    <van-nav-bar
  title="作业详情"
  left-text="返回"
  left-arrow
  @click-left="onClickLeft"
    />
<div class="time"><van-icon name="clock" />2018-2-28</div>



<div class="navbar">
<nav-tab-bar></nav-tab-bar>
</div>

  </div>

</template>

<script>
import NavTabBar from "./NavTabBar";
import "vant/lib/vant-css/icon-local.css";

export default {
  name: "index",
  data() {
    return {
      images: [
        "http://pic35.photophoto.cn/20150514/0005018352749416_b.jpg",
        "http://pic35.photophoto.cn/20150514/0005018352749416_b.jpg",
        "http://pic35.photophoto.cn/20150514/0005018352749416_b.jpg",
        "http://pic35.photophoto.cn/20150514/0005018352749416_b.jpg"
      ],
      active: 2,
      noticeIcon: "./../assets/notice.png"
    };
  },
  components: { NavTabBar }
};
function readWork() {}
</script>

<style scoped>
.time{
    float: left;
}
</style>
