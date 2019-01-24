<template>
  <div>
    <detail-banner></detail-banner>
    <detail-baseinfo></detail-baseinfo>
    <detail-header></detail-header>
    <div class="content"></div>
  </div>
</template>

<script>
import DetailBanner from './components/Banner'
import DetailHeader from './components/Header'
import DetailBaseinfo from './components/Baseinfo'
export default {
  name: 'Detail',
  components: {
    DetailBanner,
    DetailHeader,
    DetailBaseinfo
  }
}
</script>

<style lang="stylus" scoped>
  .content
    height 50rem

</style>
