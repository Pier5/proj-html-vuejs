<template>
  <div id="app">
    <HeaderRt />
    <MainRt />
    <FooterRt />
  </div>
</template>

<script>
import HeaderRt from './components/HeaderRt'
import MainRt from './components/MainRt'
import FooterRt from './components/FooterRt'

export default {
  name: 'App',
  components: {
    HeaderRt,
    MainRt,
    FooterRt
  }
}
</script>

<style lang="scss">
@import './assets/styles/style.scss';
</style>
