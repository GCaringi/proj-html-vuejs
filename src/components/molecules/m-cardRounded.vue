<template>
  <div class="relative">
    <image-page
        :source= "src"
        class="h-full"
    />
    <overlay-card
        :head = "title"
        :text = "subt"
    />
  </div>
</template>

<script>

import imagePage from '../atoms/a-imagePage.vue'
import overlayCard from '../molecules/m-cardOverlay.vue'

export default {
    name: "cardRounded",
    components: {
        imagePage,
        overlayCard,

    },
    props: {
        src: {
            type:String,
        },
        title: {
            type:String,
        },
        subt: {
            type:String,
        }
    }
}
</script>

<style>

</style>