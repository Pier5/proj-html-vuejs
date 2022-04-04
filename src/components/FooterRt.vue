<template>
  <footer>
    <div class="foot-contain">

      <!-- inserire indirizzi statici più icone social dinamiche -->
      <div class="address">
        <h3></h3>
        <h4></h4>
        <h4></h4>
        <h5></h5>
        <div class="social"></div>
      </div>

      <!-- inserire lista dinamica explore -->
      <div class="explore">
        <ul>
          <li class="title"></li>
          <li></li>
        </ul>
      </div>

      <!-- inserire lista dinamica information -->
      <div class="information">
        <ul>
          <li class="title"></li>
          <li></li>
        </ul>
      </div>

    </div>

    <!-- copyright da centrare  -->
    <div class="copyright"></div>

    <!-- cerchio verde che rimanda all'inizio della pagina -->
    <div class="circle-up"></div>

  </footer>
</template>

<script>
export default {
  name: 'FooterRt'
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";
footer {
  background-color: $hintred-color;
  .foot-contain {
    width: 900px;
    display: flex;
    position: relative;
  }
}
</style>
