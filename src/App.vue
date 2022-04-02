<template>
  <div id="app">
    <HeaderRt />
    <MainRt />
  </div>
</template>

<script>
import HeaderRt from './components/HeaderRt'
import MainRt from './components/MainRt'

export default {
  name: 'App',
  components: {
    HeaderRt,
    MainRt
  }
}
</script>

<style lang="scss">
@import './assets/styles/style.scss';
</style>
