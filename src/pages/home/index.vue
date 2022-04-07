<template>
  <view id="container">
    <view id="content">
      <header>
        <p class="goback" @click="goBaidu">&lt;</p>
        <p class="center">Hello UniApp</p>
        <p class="main">我的</p>
      </header>
      <main>
        <scroll-view scroll-x="true">
          <ul>
            <li>列表一</li>
            <li>列表二</li>
            <li>列表三</li>
            <li>列表四</li>
            <li>列表五</li>
            <li>列表六</li>
          </ul>
        </scroll-view>
      </main>
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      title: "标题",
    };
  },
  methods: {
    goBaidu() {
      location.href = "http://baidu.com";
    },
  },
  
};
</script>

<style>
#content header {
  font-size: 28rpx;
  text-align: center;
  background: #bbb;
  color: #000;
  height: 80rpx;
  line-height: 80rpx;
  display: flex;
  justify-content: space-between;
}
#content header .goback {
  width: 60rpx;
  text-align: center;
}
#content header .center {
  position: absolute;
  width: 100%;
  text-align: center;
}
#content header .main {
  width: 100rpx;
  text-align: center;
}
.animate__animated.animate__backInLeft{
  --animate-duration: 2s;
}
ul{
  overflow: hidden;
  width: 600px;
  white-space: nowrap;
}
li{
  float: left;
  width: 100px;
  height: 40px;
  list-style: none;
}
</style>