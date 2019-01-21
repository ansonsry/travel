<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1807/ad/ad574bfe6c9e1ceda3.img.png_200x200_ea7a0734.png',
        title: '成都欢乐谷',
        desc: '超级旋转过山车刺激到让你怀疑人生'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1508/53/53c486532f848d71.img.jpg_200x200_c4be246c.jpg',
        title: '成都欢乐谷',
        desc: '超级旋转过山车刺激到让你怀疑人生'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201301/16/ae96ce4058bd5cf093835fbb.jpg_200x200_e4cb9743.jpg',
        title: '成都欢乐谷',
        desc: '超级旋转过山车刺激到让你怀疑人生'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201301/16/ae96ce4058bd5cf093835fbb.jpg_200x200_e4cb9743.jpg',
        title: '成都欢乐谷',
        desc: '超级旋转过山车刺激到让你怀疑人生'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import "~styles/mixins.styl"
  .title
    margin-top .2rem
    line-height .8rem
    background #eee
    text-indent .2rem
  .item
    overflow hidden
    display flex
    height 1.9rem
    .item-img
      width 1.7rem
      height 1.7rem
      padding .1rem
    .item-info
      flex 1
      padding .2rem
      min-width 0
      .item-title
        line-height .54rem
        font-size .32rem
        ellipse()
      .item-desc
        line-height .4rem
        color #ccc
      .item-button
        line-height .44rem
        margin-top .16rem
        background #ff9300
        padding 0 .3rem
        border-radius .06rem
        color #fff
</style>
