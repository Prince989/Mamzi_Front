<template>
  <div class="body-container">
    <br>
    <mSwiper>

    </mSwiper>
    <br>
    <br>
    <div class="container p-4" dir="rtl">
      <h3 class="txt text-center">
        <strong>
          پیش نمایش سه بعدی و سفارش آنلاین غذا از بهترین رستوران ها و فست فود ها
        </strong>
      </h3>
      <br>
      <p class="txt text-center">
        با استفاده از وبسایت و اپلیکیشن سفارش آنلاین غذای مامزی شما میتونید به راحتی و در سریع ترین زمان ممکن غذای مورد
        علاقه‌ی خودتون رو از بهترین رستوران‌ها و فست فود‌های تهران، قم، کرج، گرگان، یزد، ارومیه و سایر شهرهای ایران
        سفارش بدین.
      </p>
    </div>

    <br>
    <br>
    <Favorites>

    </Favorites>

    <br>
    <br>
    <br>
    <br>
    <!-- MOST ORDERED RESTAURANTS -->
    <div>
      <h3 dir="rtl" class="float-right text-right txt header">
        <strong>
          پرسفارش ترین ها
        </strong>
      </h3>
      <a href="#" class="text-decoration-none float-left link-more txt d-none d-lg-block d-sm-block d-md-block">
        <i class="fas fa-angle-left"></i>
        <span>
          رستوران های بیشتر
        </span>
      </a>
    </div>
    <br>
    <br>
<!--    <div class="row m-0 d-flex justify-content-center flex-lg-nowrap Restaurant-Card-Container">
      <RestaurantCard class="col-lg-3 col-md-4 col-sm-5 col-12 m-1">

      </RestaurantCard>
      <RestaurantCard class="col-lg-3 col-md-4 col-sm-5 col-12 m-1">

      </RestaurantCard>
      <RestaurantCard class="col-lg-3 col-md-4 col-sm-5 col-12 m-1">
      </RestaurantCard>
      <RestaurantCard class="col-lg-3 col-md-4 col-sm-5 col-12 m-1">
      </RestaurantCard>
    </div> -->
    <RestaurantSwiper>

    </RestaurantSwiper>
    <br>
    <br>
    <br>
  </div>
</template>

<script>

  import MSwiper from "./mSwiper";
  import Favorites from "./Favorites";
  import RestaurantSwiper from "./RestaurantSwiper";
  export default {
    name: "mainBody",
    components: {Favorites, MSwiper,RestaurantSwiper},
  }
</script>

<style scoped>
  .body-container {
    background-color: white;
    height: 100%;
    display: block;
  }

  .header {
    margin-right: 70px;
  }

  .Restaurant-Card-Container {
    padding: 30px 70px 70px 70px;
  }
  .link-more{
    margin-left: 75px;
    font-size: 17px;
    color: #ffbb2f;
  }
</style>
