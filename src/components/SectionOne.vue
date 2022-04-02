<template>
  <section class="section-one">
    <div class="container">
      <div class="main-start">
        <h1>Learn At Your Own Pace!</h1>
        <h2>Get teamed up with people of the same will.</h2>
        <button class="main-btn">Get started for free</button>
      </div>
      <img src="../assets/img/home-6-hero-left-person.png" alt="immagine ragazza al pc" class="img-left">
      <img src="../assets/img/home-6-hero-poster-final.jpg" alt="immagine home" class="jumbo-img">
      <img src="../assets/img/icon-youtube-play.png" alt="logo yt" class="img-yt">
      <img src="../assets/img/home-6-hero-right-person.png" alt="immagine ragazza seduta a terra con pc" class="img-right">
    </div>

  </section>
</template>

<script>
export default {
  name: 'SectionOne'
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables.scss";

.section-one {
  background-color: $portgore-color;
  height: 500px;
  position: relative;
  z-index: -2;
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
      }
    }
  }
  .img-left {
    width: 19%;
    position: absolute;
    bottom: -60px;
    left: 232px;
  }
  .jumbo-img {
    width: 44%;
    border: 14px solid white;
    border-radius: 14px;
    box-shadow:  2px 8px  rgba(211, 208, 208, 0.2);
    z-index: 1;
  }
  .img-right {
    width: 10%;
    position: absolute;
    bottom: -160px;
    right: 318px;
    z-index: -1;
  }
  .img-yt {
    position: absolute;
    width: 4%;
    z-index: 1;
    bottom: 75px;
  }
}
</style>
