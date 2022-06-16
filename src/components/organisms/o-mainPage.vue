<template>
  <main>
    <about-section/>
    <shop-section/>
  </main>
</template>

<script>

import aboutSection from '../organisms/o-aboutSection.vue'
import shopSection from '../organisms/o-shopSection.vue'

export default {
    name: "mainPage",
    components: {
        aboutSection,
        shopSection,
    }
}
</script>

<style>

</style>