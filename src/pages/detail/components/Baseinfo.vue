<template>
  <div class="baseinfo">
    <div class="baseinfo-flexbox">
      <div class="baseinfo-flexbox-item-left">
        <div class="baseinfo-detail">
          <span class="baseinfo-score">4.9</span>
          <span class="baseinfo-text">分</span>
          <span class="baseinfo-desc">很棒</span>
        </div>
        <div class="baseinfo-comment">
          <span class="baseinfo-commentnuma">10762条评论</span>
          <span class="baseinfo-commentnumb">3条攻略</span>
        </div>
        <div class="iconfont baseinfo-icon">&#xe74e;</div>
      </div>
      <div class="baseinfo-flexbox-item-right border-left">
        <div>
          <span class="baseinfo-sightcard-title">景点简介</span>
        </div>
        <div>
          <span class="baseinfo-sightcard-text">开放时间、贴士</span>
        </div>
        <div class="iconfont baseinfo-right-icon">&#xe74e;</div>
      </div>

    </div>
    <div class="baseinfo-adress-top border-top">
      <div class="baseinfo-adress-txt">四川省成都市温江区万春镇天香路88号国色天乡乐园</div>
      <div class="iconfont adress-go-icon">&#xe74e;</div>
      <div class="iconfont adress-icon">&#xe600;</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DetailBaseinfo'
}
</script>

<style lang="stylus" scoped>
  .border-top
    &:before
      border-color #ccc
  .border-left
    &:before
      border-color #ccc
  .baseinfo
    overflow: hidden;
    width: 100%;
    height 2.4rem
    position: relative
    top: -.1rem
    //padding: .1rem .2rem 0 .2rem
    margin-bottom: .1rem
    background: #fff
    border-radius .1rem .1rem 0 0
    .baseinfo-adress-top
      position: relative;
      height .80rem
      padding: .2rem .2rem;
      margin-left .2rem
      margin-right .2rem
      display: flex;
      .baseinfo-adress-txt
        position relative
        height .72rem
        padding-left .4rem
        padding-right .4rem
        margin 0
        font-size .28rem
      .adress-go-icon
        position: absolute;
        right: 0;
        top: 50%;
        margin-top: -.14rem;
        color: #9e9e9e;
      .adress-icon
        display: block;
        position: absolute;
        left: 0;
        top: .16rem;
        margin-right: .2rem
        margin-top .1rem
        color: #9e9e9e;
        font-size: .36rem;
    .baseinfo-flexbox
      height .80rem
      margin-left .2rem
      margin-right .2rem
      padding: .2rem 0;
      display: flex;
      color #212121
      .baseinfo-flexbox-item-left
        position relative
        padding-left 0
        height .82rem
        width 50%
        float left
        .baseinfo-icon
          position: absolute;
          top .25rem
          right .2rem
          color: #9e9e9e;
        .baseinfo-detail
          position absolute
          .baseinfo-score
            font-size: .44rem
            color: #ff8300
            line-height: .44rem
          .baseinfo-text
            font-size: .28rem
            color: #ff8300
            line-height: .48rem
          .baseinfo-desc
            font-size: .28rem;
            color: #ff8300;
            line-height: .48rem;
            margin-left: .2rem;
        .baseinfo-comment
          font-size: .24rem;
          color: #9e9e9e;
          line-height: .32rem;
          margin-right: .2rem;
          margin-top .45rem
          .baseinfo-commentnumb
            margin-left .1rem
      .baseinfo-flexbox-item-right
        height .82rem
        width 50%
        float right
        .baseinfo-right-icon
          position: absolute;
          right 0
          color: #9e9e9e;
          top: 50%;
          margin-top: -.14rem;
        .baseinfo-sightcard-title
          font-size: .28rem;
          color: #212121;
          line-height: .48rem;
          padding-left: .3rem;
        .baseinfo-sightcard-text
          color: #9e9e9e;
          font-size: .24rem;
          padding-left: .3rem;
</style>
