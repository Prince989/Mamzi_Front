<template>
  <div class="">
    <h3 dir="rtl" class="text-right txt header">
      <strong>
        دسته های محبوب
      </strong>
    </h3>
    <br>
    <div class="favorites-container d-flex justify-content-center row m-0" dir="rtl">
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-01.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              پیتزا
            </span>
          </button>
        </div>
      </div>
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-02.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              کباب
            </span>
          </button>
        </div>
      </div>
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-03.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              سوپ
            </span>
          </button>
        </div>
      </div>
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-04.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              ساندویچ
            </span>
          </button>
        </div>
      </div>
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-05.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              غذای ایرانی
            </span>
          </button>
        </div>
      </div>
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-06.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              سوخاری
            </span>
          </button>
        </div>
      </div>
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-07.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              پاستا
            </span>
          </button>
        </div>
      </div>
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-08.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              سالاد
            </span>
          </button>
        </div>
      </div>
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-09.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              صبحانه
            </span>
          </button>
        </div>
      </div>
      <div class="card col-lg-2 col-md-3 col-sm-5 col-5 p-0 m-2">
        <div class="card-body p-0">
          <button class="btn bg-transparent p-0">
            <img src="@/static/foods-10.jpg" class="card-img">
            <span class="bottom-right text-white txt-light">
              استیک
            </span>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Favorites"
  }
</script>

<style scoped>
  img {
    border-radius: 12px;
  }
  .card {
    border-radius: 12px;
  }
  .bottom-right {
    position: absolute;
    bottom: 8px;
    right: 16px;
    font-size: 20px;
  }

  .card:hover {
    transition: margin-bottom .5s;
    box-shadow: 2px 2px 10px #000000;
  }
  .header{
    margin-right: 70px;
  }
  span {
    text-shadow: 0 0 3px #000000, 0 0 5px #000000;
  }
</style>
