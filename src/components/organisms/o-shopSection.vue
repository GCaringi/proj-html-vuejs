<template>
  <section id = "shoppers" class = "bg-[color:var(--clr-bg-secondary)] ">
    <shop-sites/>
  </section>
</template>

<script>

import shopSites from '../molecules/m-shopSites.vue'

export default {
    name: "shopSection",
    components: {
        shopSites,
    }
}
</script>

<style>

</style>