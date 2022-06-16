<template>
  <main>
    <about-section/>
    <shop-section/>
    <audiobook-section/>
  </main>
</template>

<script>

import aboutSection from '../organisms/o-aboutSection.vue'
import shopSection from '../organisms/o-shopSection.vue'
import audiobookSection from '../organisms/o-audiobookSection.vue'

export default {
    name: "mainPage",
    components: {
        aboutSection,
        shopSection,
        audiobookSection,
    }
}
</script>

<style>

</style>