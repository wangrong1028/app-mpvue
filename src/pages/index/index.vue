<template>
  <div class="home">
    <h1>home</h1>
    <!-- 背景轮播图 -->
    <!-- <swiper 
      indicator-dots="{{indicatorDots}}"
      autoplay="{{autoplay}}" 
      interval="{{interval}}" 
      duration="{{duration}}">
      <block mpvue:for="{{background}}" mpvue:key="*this">
        <swiper-item>
          
          <view class="swiper-item {{item}}"></view>
        </swiper-item>
      </block>
    </swiper> -->
    <img class="home-bg" :src="img.homeBg1">
  </div>
</template>

<script>
import img from '@/utils/img'

export default {
  
  data: {
    background: ['demo-text-1', 'demo-text-2', 'demo-text-3'],
    indicatorDots: true,
    vertical: false,
    autoplay: false,
    interval: 2000,
    duration: 500
  },

  // components: {
  //   img
  // }
}

</script>

<style scoped>
.home-bg {
  width: 100%;
  height: 528rpx;
}
</style>
