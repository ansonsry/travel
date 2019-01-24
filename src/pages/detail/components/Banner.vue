<template>
  <div>
    <div class="banner" @click="handleBannerClick">
      <img class="banner-img" src="//img1.qunarzz.com/sight/p0/1512/3a/3ab83c0358208e8d90.img.jpg_600x330_1a71c095.jpg"/>
      <div class="banner-info">
        <div class="banner-title">花水湾四季温泉谷</div>
      </div>
      <div class="banner-number">
        <span class="iconfont banner-icon">&#xe692;</span>
        <em class="banner-imgswipeicon-number">39</em>
      </div>
    </div>
    <common-gallary :imgs="imgs" v-show="showGallry" @close="handleGallaryClose"></common-gallary>
  </div>
</template>

<script>
import CommonGallary from 'common/gallary/Gallary'
export default {
  data () {
    return {
      showGallry: false,
      imgs: ['http://img1.qunarzz.com/sight/p0/201307/24/e18ce4d4bad04d91c8d65eac.jpg_r_800x800_c6a12345.jpg',
        'http://img1.qunarzz.com/sight/p0/1512/ae/aeed77ec209b1a7690.img.jpg_r_800x800_220bbcb2.jpg']
    }
  },
  name: 'DetailBanner',
  methods: {
    handleBannerClick () {
      this.showGallry = true
    },
    handleGallaryClose () {
      this.showGallry = false
    }
  },
  components: {
    CommonGallary
  }
}
</script>

<style lang="stylus" scoped>
  .banner
    position: relative;
    overflow: hidden;
    height: 0;
    width: 100%;
    padding-bottom: 55%;
    &:after
      background-image: linear-gradient(to bottom,rgba(0,0,0,0),rgba(0,0,0,.8));
      content: " ";
      display: block;
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      min-height: .6rem;
      background-color: transparent;
    .banner-img
      width 100%
    .banner-info
      position: absolute;
      right: .2rem;
      bottom: .36rem;
      left: .2rem;
      min-height: .4rem;
      .banner-title
        position: relative;
        z-index: 1;
        line-height: .4rem;
        color: #fff;
        font-size: .36rem;
        text-shadow: 0 1px 2px rgba(0,0,0,0.70);
    .banner-number
      position: absolute;
      left: .2rem;
      bottom: .86rem;
      width: 1.2rem;
      height: .4rem;
      background: rgba(0,0,0,.5);
      border-radius: .2rem;
      font-size: .24rem;
      color: #fff;
      line-height: .4rem;
      text-align: center;
      .banner-icon
        position: relative;
        top: .02rem;
      .banner-imgswipeicon-number
        margin-left .1rem
</style>
