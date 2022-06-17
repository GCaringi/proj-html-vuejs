<template>
  <div class="flex flex-col text-center bg-[color:var(--clr-base-light)]">
    <image-page
        :source= "src"
    />
    <div class= "flex flex-col items-center">
        <little-title
            :text = "title"
            class= "py-6 text-xl font-500"
        />
        <hr class = "w-[90%] pb-6">
        <medium-text
            :text = "content"
            class="px-[2rem] pb-[2rem]"
        />
    </div>
  </div>
</template>

<script>

import imagePage from '../atoms/a-imagePage.vue'
import mediumText from '../atoms/a-mediumText.vue'
import littleTitle from '../atoms/a-littleTitle.vue'

export default {
    name: "classicCard",
    props:{
        title: {
            type: String,
        },
        content: {
            type: String,
        },
        src: {
            type: String,
        }
    },
    components:{
        imagePage,
        mediumText,
        littleTitle,
    }
}
</script>

<style>

</style>