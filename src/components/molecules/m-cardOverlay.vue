<template>
  <div class = "m-overlay absolute inset-0 flex flex-col justify-end items-center">
        <large-text
            :text="head"
            class="pb-4 text-2xl" 
        />
        <hr class="w-[10%] py-3">
        <sub-title
            :text="text"
            class="text-[color:var(--clr-primary)] text-sm pb-8"
        />
  </div>
</template>

<script>

import largeText from '../atoms/a-largeText.vue'
import subTitle from '../atoms/a-subTitles.vue'

export default {
    name: "cardOverlay",
    components: {
        largeText,
        subTitle,
    },
    props: {
        head: {
            type: String,
        },
        text: {
            type: String,
        }
    }
}
</script>

<style lang = "scss" scoped>

.m-overlay{
    background: linear-gradient(0deg, rgba(0,0,0,0.8) 30%, rgba(255,255,255,0) 100%);;
}

</style>