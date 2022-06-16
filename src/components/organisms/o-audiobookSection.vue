<template>
  <section id = "audiobook">
    <div class = "w-[var(--width-lg)] m-auto">
      <audiobook-info
        class = "pt-[5rem]"
      />
    </div>
  </section>
</template>

<script>

import audiobookInfo from '../molecules/m-audiobookInfo.vue'

export default {
  naem: "audioBookSection",
  components: {
    audiobookInfo,
  }
}
</script>

<style lang = "scss" scoped>

#audiobook{
    background-image: url("@/assets/img/banner.jpg");
    background-size: cover;
    background-position: center;
}

</style>