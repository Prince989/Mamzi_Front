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
  </div>
</template>

<script>

  import MSwiper from "./mSwiper";
  import Favorites from "./Favorites";

  export default {
    name: "mainBody",
    components: {Favorites, MSwiper},
  }
</script>

<style scoped>
  .body-container {
    background-color: white;
    height: 100%;
    display: block;
  }
</style>
