<template>
  <div id="app">
    <headerHero/>
    <mainPage/>
  </div>
</template>

<script>

import headerHero from './components/organisms/o-headerHero.vue'
import mainPage from './components/organisms/o-mainPage.vue'

export default {
  name: 'App',
  components: {
    headerHero,
    mainPage,
  }
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";

</style>
