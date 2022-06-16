<template>
  <header class="w-[var(--width-xxl)] m-auto relative flex justify-between">
    <logo-page
      class="relative -left-[102.5px]"
    />
    <nav-bar/>
  </header>
</template>

<script>

import logoPage from '../atoms/a-logoPage.vue'
import navBar from '../molecules/m-navBar.vue'

export default {
  name: "headerPage",
  components: {
    logoPage,
    navBar,
  }
}
</script>

<style lang = "scss" scoped>

</style>