<template>
  <section class="section-two">
    <div class="circle circle-one"></div>
    <div class="circle circle-two"></div>
    <div class="circle circle-three"></div>
    <div class="circle circle-four"></div>
    <div class="circle circle-five"></div>
    <div class="circle circle-six"></div>
    <div class="circle circle-seven"></div>
    <div class="circle circle-eight"></div>
    <div class="patterns">
      <div class="pattern"></div>
      <div class="quote">
        <h1>Let passion and determination be the guide along the way and develop at your own pace that's comfortable.</h1>
        <h3>Fannie Moreno</h3>
        <h4>/Founder & Ceo</h4>
        <div class="statistics">
          <div class="single-statistic">
            <h2>1.926</h2>
            <h4>Finished sessions</h4>
          </div>
          <div class="single-statistic">
            <h2>3.092+</h2>
            <h4>Enrolled learners</h4>
          </div>
          <div class="single-statistic">
            <h2>200</h2>
            <h4>Online instructors</h4>
          </div>
          <div>
            <h2>100%</h2>
            <h4>Satisfaction rate</h4>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'SectionTwo'
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";

.section-two {
  margin-top: 60px;
  background-color: $white-color;
  background-image: url("../assets/img/background-pattern-grid-line.png");
  background-size: 270px;
  background-position-x: center;
  position: relative;
  overflow: hidden;
  .circle {
    position: absolute;
    border-radius: 50%;
  }
  .circle-one {
    width: 40px;
    height: 40px;
    background-color: $anzac-color;
    left: 150px;
    bottom: 200px;
  }
  .circle-two {
    width: 30px;
    height: 30px;
    background-color: #fa7d61;
    bottom: 360px;
    left: 350px;
  }
  .circle-three {
    width: 40px;
    height: 40px;
    background-color: transparent;
    border: 5px solid #bce6df;
    top: 40px;
    left: 320px;
  }
  .circle-four {
    width: 30px;
    height: 30px;
    background-color: $mandy-color;
    right: 350px;
    top: 230px;
  }
  .circle-five {
    width: 25px;
    height: 25px;
    background-color: #aab8f1;
    right: 470px;
    bottom: 320px;
  }
  .circle-six {
    width: 45px;
    height: 45px;
    background-color: transparent;
    border: 7px solid #f6b9aa;
    bottom: 180px;
    right: 400px;
  }
  .circle-seven {
    width: 20px;
    height: 20px;
    background-color: #bc71fe;
    top: 120px;
    left: 660px;
  }
  .circle-eight {
    width: 32px;
    height: 32px;
    background-color: #bce6df;
    top: -15px;
    right: 350px;
  }
  .quote {
    margin-top: 200px;
    width: 560px;
    text-align: center;
    display: flex;
    flex-direction: column;
    h1 {
      margin: 0 40px;
      font-size: 1.4rem;
      line-height: 2rem;
    }
    h3 {
      text-transform: uppercase;
      margin-top: 30px;
      font-size: .7rem;
    }
    h4 {
      margin-top: 10px;
      color: $silver-color;
      font-size: .7rem;
    }
    .statistics {
      display: flex;
      margin-top: 100px;
      .single-statistic {
        margin-right: 40px;
      }
      h2 {
        color: $mountain-meadow;
        font-family: 'Montserrat', sans-serif;
        font-size: 1.7rem;
        font-weight: 600;
      }
      h4 {
        width: 110px;
        color: $dovegray-color;
        font-size: .8rem;
        font-weight: lighter;
      }
    }
  }
}
</style>
