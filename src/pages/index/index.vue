<template>
  <view class="main">
    <view class="uni-margin-wrap">
      <swiper
        class="swiper"
        circular
        :indicator-dots="indicatorDots"
        :autoplay="autoplay"
        :interval="interval"
        :duration="duration"
      >
        <swiper-item>
          <view class="swiper-item uni-bg-red">
            <image class="img" src="/static/1.jpg" />
          </view>
        </swiper-item>
        <swiper-item>
          <view class="swiper-item uni-bg-green">
            <image class="img" src="/static/2.jpg" />
          </view>
        </swiper-item>
        <swiper-item>
          <view class="swiper-item uni-bg-blue">C</view>
        </swiper-item>
      </swiper>
    </view>

    <view class="icons">
      <view class="icon">
        <image src="/static/news.png" />
        <text class="iconText">志愿新闻</text>
      </view>
      <view class="icon">
        <image src="/static/team.png" />
        <text class="iconText">志愿新闻</text>
      </view>
      <view class="icon">
        <image src="/static/news.png" />
        <text class="iconText">志愿新闻</text>
      </view>
      <view class="icon">
        <image src="/static/enlarge.png" />
        <text class="iconText">志愿新闻</text>
      </view>
    </view>

    <view class="jianbianBtn"> </view>

    <Bar title="新闻展示" color="#ffa55e" />

    <Bar title="团队展示" color="#57a6ff" />
    <Bar title="活动展示" color="#8888ff" />
  </view>
</template>

<script>
import Bar from "@/components/bar/Bar.vue";

export default {
  components: {
    Bar,
  },
  data() {
    return {
      background: ["color1", "color2", "color3"],
      indicatorDots: true,
      autoplay: true,
      interval: 2000,
      duration: 500,
    };
  },
  methods: {},
};
</script>

<style scoped>
.main {
  height: 2000px;
}

.uni-margin-wrap {
  width: 690rpx;
  margin: 0 30rpx;
}
.swiper {
  height: 250rpx;
}
.swiper-item {
  display: block;
  height: 300rpx;
  line-height: 300rpx;
  text-align: center;
}

.swiper-item image {
  border-radius: 20rpx;
  width: 100%;
  height: 100%;
}
.swiper-list {
  margin-top: 40rpx;
  margin-bottom: 0;
}
.icons {
  display: flex;
  justify-content: space-around;
  padding-left: 80rpx;
  padding-right: 80rpx;
  padding-top: 40rpx;
  padding-bottom: 30rpx;
}

.icon {
  display: flex;
  flex-direction: column;
}

.icons .icon image {
  margin-left: 50%;
  transform: translateX(-50%);
  margin-bottom: 10rpx;
  width: 45rpx;
  height: 55rpx;
}

.iconText {
  font-size: 20rpx;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
}

.jianbianBtn {
  width: 90%;
  margin: 0 auto;
  height: 60rpx;
  background-image: linear-gradient(
    to right,
    rgb(255, 155, 76),
    rgb(255, 117, 117)
  );
  border-radius: 14rpx;
}
</style>
