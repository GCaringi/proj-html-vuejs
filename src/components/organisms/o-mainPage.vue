<template>
  <main>
    <about-section/>
    <shop-section/>
    <audiobook-section/>
    <critics-section/>
    <up-coming-events/>
  </main>
</template>

<script>

import aboutSection from '../organisms/o-aboutSection.vue'
import shopSection from '../organisms/o-shopSection.vue'
import audiobookSection from '../organisms/o-audiobookSection.vue'
import criticsSection from '../organisms/o-criticsSection.vue'
import upComingEvents from '../organisms/o-upcomingEvents.vue'

export default {
    name: "mainPage",
    components: {
        aboutSection,
        shopSection,
        audiobookSection,
        criticsSection,
        upComingEvents,
    }
}
</script>

<style>

</style>