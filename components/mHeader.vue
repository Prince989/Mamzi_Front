<template>
  <div class="mHeader">
    <div class="row mheaderT txt flex-nowrap">
      <div class="col-2 d-flex align-items-center justify-content-start">
        <button class="btn bg-transparent p-0 ml-4">
          <img src="@/static/buyIcon.png" height="40px" class="w-auto">
        </button>
      </div>
      <div class="col-8 align-items-center d-flex justify-content-center">
        <!--        <img src="@/static/mamzi_logo.png" height="50px" class="w-auto header-logo">-->
        <a href="#" class="header-logo"></a>
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
<!--    <br>-->
    <div class="d-flex align-items-center justify-content-center mheaderBT">
      <a href="#" class="text-decoration-none text-dark marker_txt">
        <i class="fas fa-angle-down text-danger"></i>
          <span class="txt">
          در محدوده
          </span>
          <span class="text-danger txt">
            تهران
          </span>
          <i class="fas fa-map-marker-alt text-dark"></i>
      </a>
    </div>
  </div>
</template>

<script>
  export default {
    name: "mHeader"
  }
</script>

<style scoped>
  .mHeader {
    height: 150px;
    width: 100%;
    background-color: #ffffff;
    box-shadow: 2px 2px 1px rgb(40, 40, 40);
    /*position: fixed;*/
  }

  * {
    /*padding: 0 !important;*/
    /*margin: 0!important;*/
    /*font-family: "IRANSans Light";*/
  }

  .txt {
    font-family: "IRANSans Medium"
  }

  .marker_txt {
    font-size: 18px;
  }

  .header-logo {
    background: url("@/static/mamzi_logo.png");
    height: 50px;
    background-size: cover;
    width: 169px;
  }

  .buyIcon {
    /*box-shadow: 1px 1px 1px rgba(166, 166, 166, 0.79);*/
  }

  .mheaderT {
    height: 50%;
  }
  .mheaderBT {
    height: 40%;
  }
  @media only screen and (max-width: 600px) {
    .header-logo {
      background: url("@/static/mamzi_logo_responsive.png");
      height: 50px;
      background-size: cover;
      width: 75px;
    }
  }

  @media only screen and (max-width: 940px) {
    .signup {
      display: none;
    }
    .mHeader{
      height: 110px;
    }
  }
</style>
