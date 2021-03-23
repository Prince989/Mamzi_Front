<template>
  <div class="search-background d-flex align-items-center justify-content-center">
    <div class="search-btn-Container">
      <button class="search-btn btn">
        جستجو
      </button>
    </div>
    <div class="search-field d-flex justify-content-center align-items-center p-3">
      <input type="text" class="form-control text-right bg-transparent border-0 txt" dir="rtl" placeholder="جستجوی رستوران یا غذا ...">
      <i class="fas fa-search float-right search-icon"></i>
    </div>
  </div>
</template>

<script>
  export default {
    name: "SearchBar"
  }
</script>

<style scoped>
  .search-background {
    background-color: rgba(245, 245, 245, 0.96);
    height: 110px;
    width: auto;
  }
  .search-btn-Container{
    height: 75%;
    width:150px;
    margin-top:auto;
    float: left;
  }
  .search-btn{
    background: url("@/static/SearchBtn.png") no-repeat;
    background-size: contain;
    display: block;
    height: 100%;
    width: 100%;
    border:none;
    color: transparent;
  }
  .search-field{
    background-color: white;
    border:#dddddd 1px solid;
    border-radius: 5px;
    height: 65px;
    width: 70%;
    margin-left: 10px;
  }
  .search-field input{
    font-size: 20px;
  }
  .search-field input::placeholder{
    color: #c3c3c3;
  }
  .txt{
    font-family: "IRANSans Medium";
  }
  .search-icon{
    font-size:17px;
  }
  @media only screen and (max-width: 940px){
    .search-btn{
      background: url("@/static/SearchBtn-responsive.png") no-repeat;
      background-size: contain;
      font-size: 22px;
      /*color: transparent;*/
    }
    .search-btn-Container{
      height: 75%;
      /*width: 70px;*/
      width: auto;
      margin-bottom: 2px ;
      /*width:75%;*/
    }
    .search-background{
      height: 60px;
      width: auto;
    }
    .search-field{
      height: 70%;
    }
    .search-field input{
      font-size: 16px !important;
    }
  }
</style>
