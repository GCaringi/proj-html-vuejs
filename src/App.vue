<template>
  <div id="app">
    <headerHero/>
    <mainPage/>
    <footerPage/>
  </div>
</template>

<script>

import headerHero from './components/organisms/o-headerHero.vue'
import mainPage from './components/organisms/o-mainPage.vue'
import footerPage from './components/organisms/o-footerPage.vue'

export default {
  name: 'App',
  components: {
    headerHero,
    mainPage,
    footerPage,
  }
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";

</style>
