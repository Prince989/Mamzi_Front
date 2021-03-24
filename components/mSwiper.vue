<template>
  <div class="swiper-container">
    <!-- Additional required wrapper -->
    <div class="swiper-wrapper">
      <!-- Slides -->
      <div class="swiper-slide">
        <img src="@/static/Swiper-img03.jpg" class="swiper-img">
      </div>
      <div class="swiper-slide" >
        <img src="@/static/Swiper-img02.jpg" class="swiper-img">
      </div>
      <div class="swiper-slide">
        <img src="@/static/Swiper-img01.jpg" class="swiper-img">
      </div>
    </div>
    <!-- If we need pagination -->
    <div class="swiper-pagination"></div>

    <!-- If we need navigation buttons -->
    <div class="swiper-button-prev text-white"></div>
    <div class="swiper-button-next text-white"></div>

    <!-- If we need scrollbar -->
    <div class="swiper-scrollbar"></div>
  </div>
</template>

<script>
  import Swiper, {Navigation, Pagination} from 'swiper'
  import 'swiper/swiper-bundle.css'

  Swiper.use([Navigation, Pagination])

  export default {
    name: "mSwiper",
    mounted() {
      new Swiper('.swiper-container', {
        loop: true,
        pagination: {
          el: '.swiper-pagination',
        },
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev',
        },
        scrollbar: {
          el: '.swiper-scrollbar',
        },
      })
    }
  }
</script>

<style scoped>
  .swiper-container {
    width: 85%;
    height: auto;
    border-radius: 20px;
    display: block;
  }
  .swiper-img{
    width: 100%;
    height: 100%;
  }
</style>
