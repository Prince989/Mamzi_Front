<template>
    <div class="searchbar-background d-flex align-items-center justify-content-center">
      <div class="searchbar row">
        <div class="col-2 p-0 m-0 d-flex justify-content-end align-items-center">
          <button class="btn btn-danger h-75">
            جستجوی رستوران ها
          </button>
        </div>
        <div class="col-10 d-flex justify-content-center align-items-center">
          <input type="text" class="form-control text-right" dir="rtl" placeholder="جستجوی رستوران یا غذا ...">
        </div>
      </div>
    </div>
</template>

<script>
    export default {
        name: "SearchBar"
    }
</script>

<style scoped>
  .searchbar-background {
    background-color: rgba(245, 245, 245, 0.96);
    height: 120px;
    width: auto;
  }
  .searchbar{
    width: 90%;
    height: 85%;
  }
  .searchbar div input{
    height: 78%;
  }
  .searchbar div button{
    height: 85%;
  }

</style>
