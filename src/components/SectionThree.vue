<template>
  <section class="section-three">
    <div class="patterns">
      <div class="pattern"></div>
      <div class="pattern"></div>
      <div class="pattern"></div>
      <div class="pattern"></div>
      <div class="info-section">

        <div class="col-left">
          <div class="col-col-left">

            <div class="col-top">
              <h2>Graphic design</h2>
              <h3>Have a passion for graphic and arts? Show your talents with confidence and self-assertiveness.</h3>
              <img class="img-info" src="../assets/img/home-6-service-image-01.png" alt="">
            </div>

            <div class="col-bottom">
              <img class="img-info-two" src="../assets/img/home-6-service-image-03.png" alt="">
              <h2>Idea discussion</h2>
              <h3>Get teamed up with the specialists who work and teach coding for years at famous universities.</h3>
            </div>

          </div>

          <div class="col-col-right">ciao</div>
        </div>

        <div class="col-right">
          ciao
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'SectionThree'
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables.scss";

.info-section{
  position: absolute;
  margin-top: 30px;
  width: 630px;
  display: flex;
  .col-left {
    display: flex;
    width: 55%;
    .col-col-left {
      width: 50%;
      .col-top,
      .col-bottom {
        height: 250px;
        margin-bottom: 20px;
      }
    }
    .col-col-right {
      width: 50%;
      margin-left: 20px;
    }
    h2 {
      padding-left: .4rem;
      font-size: .9rem;
      margin: .4rem 0;
    }
    h3 {
      padding-left: .4rem;
      font-size: .7rem;
      font-weight: lighter;
      color: $dovegray-color;
      margin-bottom: .8rem;
    }
    .img-info {
      width: 95%;
    }
    .img-info-two {
      width: 75%;
    }
  }
  .col-right {
    width: 45%;

  }
}
</style>
