<template>
  <div class="card-container">
    <div class="card txt">
      <div class="card-header p-0">
        <img src="@/static/restaurant-01.jpg" class="card-img-top">
        <i class="far fa-heart heart"></i>
      </div>
      <div class="card-body text-right" dir="rtl">
        <h4>
          شمرون کباب
        </h4>
        <div class="text-secondary txt-light">
          <small>
            <i class="fas fa-map-marker-alt"></i>
            <span>
            نیاوران
          </span>
          </small>
        </div>
      </div>
      <span class="float-left txt ml-3 text-secondary" dir="rtl">
        <small>
        (120 نظر)
      </small>
      </span>
      <StarComponent class="float-left col-2 ml-3 mb-3 text-secondary p-0">

      </StarComponent>
    </div>
  </div>
</template>

<script>
  import StarComponent from "./StarComponent";

  export default {
    name: "RestaurantCard",
    components: {StarComponent}
  }
</script>

<style scoped>
  .card-container {
    border-radius: 15px;
    box-shadow: 0 10px 25px #bbbbbb;
    padding: 0;
    cursor: pointer;
    transition: 0.2s;
  }
  .card-container:hover{
    margin-top:-5px !important;
    box-shadow: none;
  }

  .card {
    border-radius: 15px;
  }

  .card-header {
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
  }

  img {
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
  }
  .heart{
    position: absolute;
    top: 8px;
    right: 16px;
    font-size: 25px;
    color: white;
  }
</style>
