<template>
  <div class = "w-[var(--width-xxl)] m-auto relative">
    <hero-info/>
  </div>
</template>

<script>

import heroInfo from '../molecules/m-heroInfo.vue'

export default {
    name: "heroMain",
    components: {
        heroInfo,
    }
}
</script>

<style>

</style>