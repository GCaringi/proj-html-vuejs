<template>
  <div class="w-[var(--width-lg)] m-auto flex py-[3rem] justify-between">
    <image-page
    v-for = "(img, index) in imagesPath"
    :key = "index"
    :source= "img"
    />
  </div>
</template>

<script>

import imagePage from '../atoms/a-imagePage.vue'

export default {
    name: "shopSite",
    components:{
        imagePage,
    },
    data(){
        return {
            imagesPath: [
                "ebay-logotan-2x-200x66.png",
                "audible-logotan-2x-200x66.png",
                "bb-logotan-2x-200x66.png",
                "kindlefire-logotan-2x-200x66.png"
            ]
        }
    }
}
</script>

<style>

</style>