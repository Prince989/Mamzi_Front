<template>
  <div class="mHeader">
    <div class="row mheaderT txt">
      <div class="col-2 d-flex align-items-center justify-content-center">
        <button class="btn buyIcon p-0" >
          <img src="@/static/buyIcon.png"  height="35px" class="w-auto">
        </button>
      </div>
      <div class="col-8 align-items-center d-flex justify-content-center">
        <img src="@/static/mamzi_logo.png" height="50px" class="w-auto">
      </div>
      <div class="col-2 row d-flex justify-content-center align-items-center">
        <button class="btn bg-transparent signup">
          ثبت نام
        </button>
        <button class="btn btn-outline-danger">
          ورود
        </button>
      </div>
    </div>
    <hr class="m-1">
    <br>
    <div class="d-flex align-items-center justify-content-center">
      <a href="#" class="text-decoration-none text-secondary marker_txt">
        <strong>
        <span class="txt">
          در محدوده تهران
        </span>
        <i class="fas fa-map-marker-alt text-secondary"></i>
        </strong>
      </a>
    </div>
    <hr>
  </div>
</template>

<script>
    export default {
        name: "mHeader"
    }
</script>

<style scoped>
  .mHeader{
    height: 120px;
    width: 100%;
    background-color: #ffffff;
  }
  *{
    /*padding: 0 !important;*/
    /*margin: 0!important;*/
    /*font-family: "IRANSans Light";*/
  }
  .txt{
    font-family: "IRANSans Light"
  }
  .marker_txt{
    font-size:19px;
  }
  .buyIcon{
    /*height:50px;*/
    /*width: 70px;*/
  }
  .mheaderT{
    height: 50%;
  }
  @media only screen and (max-width: 600px) {
    .signup {
      display: none;
    }
  }
</style>
