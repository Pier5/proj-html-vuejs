<template>
  <section class="section-nine">
    <div class="circle-one"></div>
    <div class="circle-two"></div>
    <div class="circle-three"></div>
    <h2>Start today for getting <span class="green-text">Online Certification</span></h2>
    <h1>You can be your own guiding star with our help!</h1>
    <button class="main-btn">Get started now</button>
  </section>
</template>

<script>
export default {
  name: 'SectionNine'
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";
.section-nine {
  text-align: center;
  padding: 50px 0 80px;
  position: relative;
  .circle-one {
    position: absolute;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: $anzac-color;
    left: 80px;
    bottom: 120px;
  }
  .circle-two {
    position: absolute;
    width: 35px;
    height: 35px;
    border-radius: 50%;
    background-color: $mandy-color;
    right: 370px;
    bottom: 235px;
  }
  .circle-three {
    position: absolute;
    width: 33px;
    height: 33px;
    border-radius: 50%;
    background-color: #aab8f1;
    right: 170px;
    bottom: 120px;
  }
  h2 {
    font-size: 1rem;
    .green-text {
      color: $jungle-green;
    }
  }
  h1 {
    margin: 5px 0 20px;
  }
  .main-btn {
    border: none;
    background-color: $mountain-meadow;
    color: $white-color;
    font-weight: bolder;
    font-size: .7rem;
    padding: .6rem 2.4rem;
    border-radius: 3px;
    cursor: pointer;
    font-family: 'Quicksand', sans-serif;
    transition: .5s;
  }
  .main-btn:hover {
    background-color: #3f3a64;
    color: $mandy-color;
    transition: .5s;
  }
}
</style>
