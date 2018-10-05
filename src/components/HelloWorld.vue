<template>
  <!-- swiper -->
  <swiper :options="swiperOption" style="height: auto">
    <swiper-slide><img src="@/assets/bg.jpg" alt=""></swiper-slide>
    <swiper-slide><img src="@/assets/bg.jpg" alt=""></swiper-slide>
    <swiper-slide><img src="@/assets/bg.jpg" alt=""></swiper-slide>
    <swiper-slide><img src="@/assets/bg.jpg" alt=""></swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</template>

<script>
export default {
  data () {
    return {
      swiperOption: {
        autoHeight: true,
        loop: true,
        spaceBetween: 20,
        centeredSlides: true,
        slidesPerView: 'auto',
        // slidesPerView: 3,
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        }
      }
    }
  }
}
</script>

<style scoped>
  .swiper-container{
    margin: 0 -30px;
  }
  /*.swiper-container .swiper-slide {*/
    /*!*padding-right: 20px;*!*/
    /*margin-right: 20px;*/
  /*}*/
  .swiper-slide {
    width: 80%;
    /*padding: 10px;*/
  }
  .swiper-container .swiper-slide img{
    max-width: 100%;
    width: 100%;
  }
</style>
