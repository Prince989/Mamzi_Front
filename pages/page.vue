<template>
  <div class="baby">
    <header-t-p>

    </header-t-p>
    <header-b-t>

    </header-b-t>
  </div>
</template>

<script>
  import HeaderBT from "../components/headerBT";
  import HeaderTP from "../components/headerTP";
  export default {
    name: "page",
    components: {HeaderTP, HeaderBT}
  }
</script>

<style scoped>
  .baby{
    font-family: 'B Yekan',monospace;
    font-style: normal;
    font-size: 16px;
    font-weight: unset !important;
  }

</style>
