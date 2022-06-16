<template>
  <div id="app">
    <headerHero/>
  </div>
</template>

<script>

import headerHero from './components/organisms/o-headerHero.vue'

export default {
  name: 'App',
  components: {
    headerHero,
  }
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";

</style>
