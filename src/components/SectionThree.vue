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

          <div class="col-col-right">
            <div class="col-top">
              <h2>Business Administration</h2>
              <h3>Learners are encouraged to study the mechanism and structure of system administration.</h3>
              <img class="img-info-three" src="../assets/img/home-6-service-image-02.png" alt="">
            </div>
            <div class="col-bottom">
              <img class="img-info-four" src="../assets/img/home-6-service-image-04.png" alt="">
              <h2>Web Development</h2>
              <h3>Learn to start building a webpage from scratch. You decide your own pace, course and speed.</h3>
            </div>
          </div>
        </div>
        <div class="col-right">
          <span class="span-text">Together we can create</span>
          <h1>Service We <span class="green-text">Can Provide</span> For My Clients. </h1>
          <ul>
            <li>Select & customize courses to your preferences</li>
            <li>Change the tutor and make arrangements</li>
            <li>Partecipate in events to join others</li>
            <li>Get the desired certificate delivered at house</li>
        </ul>
        <button class="main-btn">Get started for free</button>
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
@import "../assets/styles/partials/variables";

.section-three {
  height: 550px;
}
.info-section{
  position: absolute;
  margin-top: 30px;
  width: 700px;
  display: flex;
  .col-left {
    display: flex;
    width: 55%;
    .col-col-left {
      width: 50%;
      margin-bottom: 40px;
      box-shadow: 0 3px 10px 8px rgba(211, 208, 208, 0.3);
    }
    .col-col-right {
      width: 50%;
      margin-left: 20px;
      margin-top: 40px;
      box-shadow: 0 3px 10px 8px rgba(211, 208, 208, 0.3);
    }
    .col-top,
    .col-bottom {
      margin-bottom: 25px;
      padding: .6rem .4rem 0;
    }
    .col-top {
      box-shadow: 0 3px 10px 8px rgba(211, 208, 208, 0.3);
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
      margin-bottom: .4rem;
    }
    .img-info {
      width: 90%;
    }
    .img-info-two {
      width: 65%;
    }
    .img-info-three {
      width: 65%;
      margin-left: 1.8rem;
    }
    .img-info-four {
      width: 85%;
      margin-left: 1rem;

    }
  }
  .col-right {
    width: 45%;
    padding-top: 110px;
    padding-left: 30px;
    margin-left: 10px;
    .span-text {
      font-size: .7rem;
      color: $dovegray-color;
      text-transform: uppercase;
    }
    h1 {
      margin: 1rem 0 1.6rem;
      font-size: 1.8rem;
      line-height: 2rem;
      .green-text {
        color: $mountain-meadow;
        font-weight: lighter;
      }
    }
    li {
      list-style-type: none;
      font-size: .6rem;
      color: $dovegray-color;
      line-height: 1.4rem;
      font-family: 'Questrial', sans-serif;
    }
    li::before {
      content: "\2713";
      color: $mountain-meadow;
      font-weight: bolder;
      font-size: .7rem;
      margin-right: .6rem;
    }
    .main-btn {
      border: none;
      background-color: $mountain-meadow;
      color: $white-color;
      font-weight: bolder;
      font-size: .7rem;
      padding: .6rem 1.2rem;
      border-radius: 3px;
      margin-top: 15px;
      cursor: pointer;
      font-family: 'Quicksand', sans-serif;
    }
  }
}
</style>
