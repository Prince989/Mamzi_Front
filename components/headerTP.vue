<template>
  <div class="container-fluid navbarSh">
    <div class="container align-items-center">
      <div class="justify-content-around d-flex">
        <ul class="list-inline d-flex first-nav align-content-end">
          <li><i class="fa fa-user-circle-o align-content-between" aria-hidden="true"></i><small><a href="#" class="mr-4 text-decoration-none">  &nbsp حساب من</a></small></li>
          <li><a href="#" class="text-decoration-none"><i class="fa fa-comments align-content-center" aria-hidden="true"></i>&nbsp<small> چت های من    </small></a></li>
        </ul>
        <ul class="list-inline text-right d-flex first-nav">
          <li><small><a href="#" class="text-decoration-none">پشتیبانی</a></small></li>
          <li><small><a href="#" class="ml-4 text-decoration-none">همه آگهی ها</a></small></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "headerTP"
    }
</script>

<style scoped>
  .navbarSh {
    height: 30px !important;
    background: rgba(235, 235, 235, 0.85);
    border : none;
    border-radius: 0px;
  }
  .first-nav li a{
    color: #828283;
  }
  .first-nav li{
    color: #828283;
  }
  .first-nav li a:hover{
    color: #ff9300 !important;
    text-decoration: none;
  }
  @media only screen and (max-width: 600px) {
    .navbarSh {
      display: none;
    }
  }
</style>
