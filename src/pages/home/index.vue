<template>
  <view id="container">
      <view id="content">
        <header>
          <p class="goback" @click="goBaidu">&lt;</p>
          <p class="center">Hello UniApp</p>
          <p class="main">我的</p>
        </header>
        <main>

        </main>
      </view>
  </view>
</template>

<script>
export default {
  methods:{
    goBaidu() {
      location.href = 'http://baidu.com'
    }
  }
}
</script>

<style>
#content header{
  font-size: 3.5vw;
  text-align: center;
  background: #bbb;
  color: #000;
  height: 5vh;
  line-height: 5vh;
  display: flex;
  justify-content: space-between;
}
#content header .gobaack{
  width: 2vw;
  text-align: center;
  font-weight: bold;
}
#content header .center{
  position: absolute;
  width: 100%;
  text-align: center;
}
#content header .main{
  width: 10vw;
  text-align: center;
}
</style>