<template>
  <main>
    <SectionOne />
    <SectionTwo />
    <SectionThree />
    <SectionFour />
    <SectionFive />
    <SectionSix />
  </main>
</template>

<script>
import SectionOne from './SectionOne.vue'
import SectionTwo from './SectionTwo.vue'
import SectionThree from './SectionThree.vue'
import SectionFour from './SectionFour.vue'
import SectionFive from './SectionFive.vue'
import SectionSix from './SectionSix.vue'

export default {
  name: 'MainRt',
  components: {
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    SectionSix
  }
}
</script>

<style lang="scss" scoped>

</style>
