<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide class="index_swiper" v-for="item of swiperList" :key="item.id">
        <img
          class="index_banner"
          :src="item.imgSrc"
          alt
        >
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data: function () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop:true
      },
      swiperList: [{
        id:"0001",
        imgSrc:"http://img1.qunarzz.com/piao/fusion/1609/1b/371522f509580f02.jpg_750x200_8d978cde.jpg"
      },{
        id:"0002",
        imgSrc:"http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20196/b2816bed3f46772d0ba57decd833bc0a.jpg_750x200_0517517a.jpg"
      },{
        id:"0003",
        imgSrc:"http://img1.qunarzz.com/piao/fusion/1610/f3/f39d9de1e92deb02.jpg_750x200_8cbc3f9b.jpg"
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
.wrapper >>>.swiper-pagination-bullet-active
  background #ffffff !important
.wrapper
  overflow hidden
  width 100%
  height 0
  padding-bottom 26.667%
  background #eeeeee
  .index_banner
    width: 100%
</style>
