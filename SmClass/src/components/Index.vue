<template>

  <div class="mx">
    <van-nav-bar title="首页" fixed=true></van-nav-bar>

<div>
<van-swipe :autoplay="3000">
  <van-swipe-item v-for="(image, index) in images" :key="index">
    <img v-bind:src="image" width="400px">
  </van-swipe-item>
</van-swipe>

<van-notice-bar
  text="足协杯战线连续第2年上演广州德比战，上赛季半决赛上恒大以两回合5-3的总比分淘汰富力。"
  left-icon='./../assets/notice.png'/>

<div class="card" @click="readWork">
    <div class="classname"><b><van-icon name="description" /><b class="setcname">高数</b></b></div>
    <div><b><van-icon name="question" class="sicon"/></b><font class="setcname">马巧梅 18235462547</font></div>
    <div><van-icon name="clock" class="sicon" /><font class="setcname">2018-2-28</font></div>
</div>
<div class="card">
  <div class="classname"><b><van-icon name="description" /><b class="setcname">高数</b></b></div>
  <div><van-icon name="question" class="sicon" />  马巧梅 18235462547</div>
  <div><van-icon name="clock"  class="sicon"/>  2018-2-28</div>
</div>


</div>

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
function readWork(){

}
</script>

<style scoped>
.mx {
  width: 100%;
  height: 100%;
}

.navbar {
  margin-top: 20%;
}
.card {
  padding-top: 8px;
  padding-left: 15px;
  padding-bottom: 7px;
  box-shadow: 0 0px 8px 0 rgba(0, 0, 0, 0.2);
  border-radius: 9px;
  margin-top: 5px;
  color: rgb(100, 100, 100);
  border-right:10px solid rgb(43, 255, 0);
  /* border-right:10px solid #FF0000; */
}
.classname {
  padding: 0 0 3px 0;
  font-size: 20px;
}
.setcname {
  padding-left: 5px;
}
.sicon {
  color: rgb(22, 145, 216);
}

</style>
