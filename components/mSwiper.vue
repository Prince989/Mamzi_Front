<template>
  <div class="swiper-container swiper1">
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
    <div class="swiper-pagination pagination1"></div>

    <!-- If we need navigation buttons -->
    <div class="swiper-button-prev text-white"></div>
    <div class="swiper-button-next text-white"></div>

    <!-- If we need scrollbar -->
<!--    <div class="swiper-scrollbar"></div>-->
  </div>
</template>

<script>
  import Swiper, {Navigation, Pagination} from 'swiper'
  import 'swiper/swiper-bundle.css'

  Swiper.use([Navigation, Pagination]);

  export default {
    name: "mSwiper",
    data() {
      return {
        windowWidth: 0
      }
    },
    mounted() {
      new Swiper('.swiper1', {
        loop: true,
        pagination: {
          el: '.pagination1',
        },
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev',
        },
        scrollbar: {
          el: '.swiper-scrollbar',
        },
      });
    }
  }
</script>

<style scoped>
  .swiper1 {
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
