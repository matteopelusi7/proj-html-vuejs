<template>
  <div id="app">
    <MainHeader />
    <MainContent />
    <FooterContent />
  </div>
</template>

<script>

import MainHeader from './components/Header.vue'
import MainContent from './components/Main.vue'
import FooterContent from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    FooterContent
  }
}
</script>

<style lang="scss">

@import './assets/scss/common.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

</style>
