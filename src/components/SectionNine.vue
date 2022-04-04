<template>
  <section class="section-nine">
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
      padding: .6rem 2rem;
      border-radius: 3px;
      cursor: pointer;
      font-family: 'Quicksand', sans-serif;
    }
}
</style>
