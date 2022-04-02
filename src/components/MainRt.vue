<template>
  <main>
    <SectionOne />
    <SectionTwo />
    <SectionThree />
  </main>
</template>

<script>
import SectionOne from './SectionOne.vue'
import SectionTwo from './SectionTwo.vue'
import SectionThree from './SectionThree.vue'

export default {
  name: 'MainRt',
  components: {
    SectionOne,
    SectionTwo,
    SectionThree
  }
}
</script>

<style lang="scss" scoped>

</style>
