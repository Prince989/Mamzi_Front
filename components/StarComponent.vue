<template>
    <div class="d-flex justify-content-center ">
      <span class="fas fa-star f-size checked"></span>
      <span class="fas fa-star f-size checked"></span>
      <span class="fas fa-star f-size checked"></span>
      <span class="fas fa-star f-size checked"></span>
      <span class="fas fa-star f-size "></span>
    </div>
</template>

<script>
    export default {
        name: "StarComponent"
    }
</script>

<style scoped>
  .f-size{
    font-size: 11px;
  }
  .checked{
    color: #ffd11b;
  }
</style>
