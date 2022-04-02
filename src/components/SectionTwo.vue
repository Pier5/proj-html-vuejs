<template>
  <section class="section-two">
    <div class="patterns">
      <div class="pattern"></div>
      <div class="pattern"></div>
      <div class="pattern"></div>
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
@import "../assets/styles/partials/variables.scss";

.section-two {
  margin-top: 60px;
  background-color: $white-color;
  .quote {
    position: absolute;
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
        font-size: 1.4rem;
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
