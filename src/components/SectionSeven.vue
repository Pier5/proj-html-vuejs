<template>
  <section class="section-seven">
    <div class="section-bridge">
      <div class="bridge-text">Wanna transform your life?</div>
      <h1>Glad to <span class="green-text">Help You</span> Learn</h1>
    </div>
  </section>
</template>

<script>
export default {
  name: 'SectionSeven'
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/partials/variables";

.section-bridge {
    text-align: center;
    margin: 0 auto;
    .bridge-text {
      font-size: .7rem;
      color: $dovegray-color;
      text-transform: uppercase;
      padding-top: 50px
    }
    h1 {
      margin: 1rem 0 2.5rem;
      font-size: 1.9rem;
      line-height: 2rem;
      .green-text {
        color: $mountain-meadow;
        font-weight: lighter;
      }
    }
}
</style>
