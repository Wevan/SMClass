<template>

  <div class="mx">
    <van-nav-bar
  title="作业详情"
  left-text="返回"
  left-arrow
  @click-left="onClickLeft"
    />
<div class="card">
    <div class="classname"><b><van-icon name="description" /><b class="setcname">高数</b></b></div>
    <div><b><van-icon name="question" class="sicon"/></b><font class="setcname">马巧梅 18235462547</font></div>
    <div><van-icon name="clock" class="sicon" /><font class="setcname">2018-2-28</font></div>
</div>
<div class="card">
１．函数ｙ＝ａｒｃｓｉｎ√１－ｘ2 ＋ ────── 的定义域为 _________。
２．函数ｙ＝ｘ＋ｅx 上点（ ０，１ ）处的切线方程是______________。
３．设ｆ（X）在Xo 可导且ｆ'（Xo）＝Ａ，则ｌｉｍ  h→o h ＝ _____________。
</div>
<div class="swtype">
  <van-icon name="photograph" class="sicon" />&nbsp;&nbsp;&nbsp;<van-icon name="play"  class="sicon"/>
</div>

<div class='textarea-wrapper'>
	<div class='textarea-block'>
		<textarea class="textarea-item" name="content" placeholder="请输入文本作答内容" maxlength="5000" spellcheck="false"></textarea>
	</div>
	<van-button size="large" type="primary">提交</van-button>
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
function readWork() {}
</script>

<style scoped>
.card {
  padding-top: 8px;
  padding-left: 15px;
  padding-bottom: 7px;
  box-shadow: 0 0px 8px 0 rgba(0, 0, 0, 0.2);
  border-radius: 9px;
  margin-top: 5px;
  color: rgb(100, 100, 100);
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
.swtype {
  font-size: 30px;
  text-shadow: 0 0px 8px 0 rgba(0, 0, 0, 0.2);
  padding: 2px 0 2px 5px;
}
.textarea-wrapper {
  width: 100%；;
}
.textarea-block {
  position: relative;
}
.textarea-item {
  width: 100%;
  height: 160px;
  border: 1px solid #ccc;
  padding: 10px;
  resize: none;
  color: #aaa;
}
.navbar {
  margin-top: 20%;
}
.time {
  float: left;
}
</style>
