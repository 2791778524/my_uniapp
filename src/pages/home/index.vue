<template>
  <view id="container">
    <view id="content">
      <header>
        <p class="goback" @click="goBaidu">&lt;</p>
        <p class="center">Hello UniApp</p>
        <p class="main">我的</p>
      </header>
      <main>
        {{ title }}
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
  onLoad() {
    console.log(uni.getSystemInfoSync().statusBarHeight);
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
</style>