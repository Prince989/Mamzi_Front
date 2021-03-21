<template>
  <div>
    <div class="row flex-row-reverse headerbt-m d-flex  align-items-center p-0">
      <div class="col-10 h-75 d-flex align-items-center justify-content-center m-0 p-0">
        <div class="searchfield row d-flex flex-row-reverse m-0">
          <div class="row m-0 col-8 p-0">
            <div class="col-10 d-flex align-items-center p-0">
              <input type="text" class="form-control bg-transparent border-0 text-sm-right p-1" placeholder="جستجو..."
                     dir="rtl">
            </div>
            <div class="col-2 p-0 d-flex align-items-center justify-content-center">
              <button class="btn d-flex p-0">
                <i class="fas fa-bars text-secondary"></i>
              </button>
            </div>
          </div>
          <div class="row m-0 col-4 p-0">
            <div class="col-4 p-0 m-0 d-flex align-items-center justify-content-center">
              <i class="fas fa-map-marker-alt text-secondary marker" style="font-size: 15px"></i>
            </div>
            <div class="col-8 p-0 m-0 text-nowrap text-secondary align-items-center d-flex">
              <span style="font-size: 13px">
                همه ایران
              </span>
            </div>
          </div>
          <!--          <div class="col-3 row d-flex flex-row-reverse flex-nowrap align-items-center">-->
          <!--            <small class="col-6 w-auto ">-->
          <!--              <label class="text-secondary text-center text-nowrap position-static">همه ایران</label>-->
          <!--            </small>-->
          <!--            <i class="fas fa-map-marker-alt text-secondary col-6"></i>-->
          <!--          </div>-->
        </div>
      </div>
      <div class="col-2 align-items-center d-flex justify-content-end p-0 m-0">
        <button class="btn m-0 p-0 d-flex justify-content-center" style="font-size: 19px">
          <i class="fa fa-comments align-content-center text-secondary text-right" aria-hidden="true"></i>
        </button>
      </div>
    </div>
    <div class="headerbt">
      <div class="container h-100 d-flex align-items-center pr-5 pl-5">
        <button class="btn btn-info addbtn d-flex align-items-center" style="font-size: medium"> ثبت آگهی رایگان &nbsp;
          &nbsp;<i
            class="fas fa-plus"></i></button>
        <img src="@/static/mamzi.png" class="d-flex ml-auto" width="76" height="43">
      </div>
      <br>
      <div class="container text-right text-dark" dir="rtl">
        <h4>
          نیازمندی های رایگان بینگو
        </h4>
        <p>
          خرید و فروش خودرو، املاک، آپارتمان، گوشی موبایل، تبلت، لوازم خانگی، لوازم دست دوم، استخدام و هر چه فکر کنید!
        </p>
      </div>
      <br><br>
      <div class="container filter form-group row m-auto align-items-center d-flex flex-row-reverse">
        <div class="col-5" dir="rtl">
          <input type="search" class="form-control text-right " placeholder="جستجو...">
        </div>
        <div class="col-3" dir="rtl">
          <select class="form-control">
            <option>
              همه گروه ها
            </option>
            <option>
              ماشین
            </option>
            <option>
              مسکن
            </option>
          </select>
        </div>
        <div class="col-3">
          <select class="form-control" dir="rtl">
            <option>
              همه گروه ها
            </option>
            <option>
              ماشین
            </option>
            <option>
              مسکن
            </option>
          </select>
        </div>
        <div class="col-1">
          <button class="btn btn-primary w-100 d-flex align-items-center"><span>جستجو</span> &nbsp;&nbsp; <i
            class="fas fa-search"></i></button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "headerBT"
  }
</script>

<style scoped>
  .headerbt {
    height: 55px;
    color: rgba(234, 248, 255, 0.85);
    box-shadow: rgba(78, 85, 91, 0.22) 1px 1px 1px 0.8px;
  }

  .col-5 {
    padding: 0px;
    margin: 0px;
  }

  .col-3 {
    padding: 0px;
    margin: 0px;
  }

  .col-1 {
    padding: 0px;
    margin: 0px;
  }

  .container {
    padding-right: 50px;
    padding-left: 50px;
  }

  .headerbt-m {
    height: 60px;
    color: rgba(234, 248, 255, 0.85);
    box-shadow: 1px 0.1px 5px rgba(78, 85, 91, 0.19);
  }

  .filter {
    background-color: #ffffff;
    height: 70px;
    box-shadow: 1px 1px 10px rgba(78, 85, 91, 0.19);
    border-radius: 5px;
  }

  .filter div select {
    border-radius: 0;
  }

  .filter div button {
    border-radius: 5px 0 0 5px;
  }

  .filter div input {
    border-radius: 0 5px 0 0;
  }

  @media only screen and (max-width: 600px) {
    .headerbt {
      display: none;
    }
  }

  @media only screen and (min-width: 601px) {
    .headerbt-m {
      display: none !important;
    }
  }

  .searchfield {
    border-radius: 7px;
    height: 85%;
    width: 80%;
    background-color: #eeeeee;
  }

  .searchfield div div input {
    font-size: small;
  }

  .searchfield div div input:hover {
    box-shadow: none;
  }

  .searchbar {
    background-color: #eeeeee;
    box-shadow: none;
    border-radius: 7px;
    height: 85%;
  }

  .searchbar input {
    border: none;
    background: none;
    outline: none;
    padding: 0;
    font-size: 12px;
  }

  .searchbar input:focus {
    outline: none;
    box-shadow: none;
  }

  .addbtn {
    border-radius: 16px;
    margin-top: auto;
    margin-bottom: auto;
    font-size: smaller;
    background-color: #0084ff;
  }

  .marker {
    font-size: 19px;
  }

</style>
