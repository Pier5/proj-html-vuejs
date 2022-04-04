<template>
  <section class="section-one">
    <div class="container">
      <div class="main-start">
        <h1>Learn At Your Own Pace!</h1>
        <h2>Get teamed up with people of the same will.</h2>
        <button class="main-btn">Get started for free</button>
        <div class="img-container">
          <img class="img-left" src="../assets/img/home-6-hero-left-person-244x300.png" alt="">
          <img class="img-middle" src="../assets/img/home-6-hero-poster-final.jpg" alt="">
          <img class="img-over-middle" src="../assets/img/icon-youtube-play.png" alt="">
          <img class="img-right" src="../assets/img/home-6-hero-right-person.png" alt="">
        </div>
      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'SectionOne'
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";

.section-one {
  background-color: $portgore-color;
  height: 500px;
  position: relative;
  .container {
    justify-content: center;
    flex-direction: column;
    .main-start {
      margin-top: 50px;
      text-align: center;
      h1 {
        color: $white-color;
        font-size: 2.2rem;
        margin-top: 20px;
        margin-bottom: 12px;
      }
      h2 {
        color: $silver-color;
        font-size: .8rem;
        margin-bottom: 25px;
      }
      .main-btn {
      border: none;
      background-color: $mountain-meadow;
      color: $white-color;
      font-weight: bolder;
      font-size: .7rem;
      padding: .6rem 1.2rem;
      border-radius: 3px;
      margin-bottom: 60px;
      font-family: 'Quicksand', sans-serif;
      }
    }
    .img-container {
      width: 100%;
      margin: 30px auto 0;
      position: relative;

      .img-left {
        float: left;
        width: 25%;
        position: relative;
        bottom: 50px;
        left: 35px;
        z-index: 0;
      }
      .img-middle {
        float: left;
        width: 50%;
        border: 12px solid $white-color;
        border-radius: 4px;
        position: relative;
        bottom: 45px;
        z-index: 1;
      }
      .img-over-middle {
        position: absolute;
        bottom: -140px;
        right: 500px;
        width: 55px;
        z-index: 2;
      }
      .img-right {
        float: left;
        width: 12%;
        position: relative;
        bottom: -170px;
        z-index: 0;
      }
    }
  }
}
</style>
