<template>
  <main>
    <SectionOne />
    <SectionTwo />
    <SectionThree />
    <SectionFour />
    <SectionFive />
    <SectionSix />
    <SectionSeven />
    <SectionEight />
    <SectionNine />
  </main>
</template>

<script>
import SectionOne from './SectionOne.vue'
import SectionTwo from './SectionTwo.vue'
import SectionThree from './SectionThree.vue'
import SectionFour from './SectionFour.vue'
import SectionFive from './SectionFive.vue'
import SectionSix from './SectionSix.vue'
import SectionSeven from './SectionSeven.vue'
import SectionEight from './SectionEight.vue'
import SectionNine from './SectionNine.vue'

export default {
  name: 'MainRt',
  components: {
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    SectionSix,
    SectionSeven,
    SectionEight,
    SectionNine
  }
}
</script>

<style lang="scss" scoped>

</style>
