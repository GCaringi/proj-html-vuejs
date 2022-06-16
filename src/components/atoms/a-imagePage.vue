<template>
  <img :src="require('@/assets/img/' + source)" alt="Imagine">
</template>

<script>
export default {
    name: "imagePage",
    props: {
      source: {
        type: String,
        required: true,
      }
    }
}
</script>

<style>

</style>