<template>
  <div class = "flex">
    <div class="w-1/2">
        <image-page
            source= "audible-app-2x-400x418.png"
        />
    </div>
    <div class = "w-1/2 flex flex-col items-center justify-center text-center text-center">
        <large-text
            text = "New Audiobook"
            class = "text-[2.5rem]"
        />
        <sub-title
            text = "No time to read? No problem listen to it"
            class = "text-[color:var(--clr-primary)] text-xl pb-4"
        />
        <little-text
            text = "Donec fringilla nunc eu turpis dignissim, at euismod sapien ticidunt. Maecenas eleifend congue cursus"
            class = "text-[color:var(--clr-typo-secondary)] text-lg px-[1rem] pb-4"
        />
        <div class=" w-full flex justify-between pt-4">
            <image-page
                v-for = "(logo, index) in logoList"
                :key = "index"
                :source= "logo"
            />
        </div>
    </div>
  </div>
</template>

<script>

import imagePage from '../atoms/a-imagePage.vue'
import largeText from '../atoms/a-largeText.vue'
import subTitle from '../atoms/a-subTitles.vue'
import littleText from '../atoms/a-littleText.vue'

export default {
    name: "audiobookInfo",
    components: {
        imagePage,
        largeText,
        subTitle,
        littleText,
    },
    data(){
        return {
            logoList: [
                "audible-logo.png",
                "bn-logo-tall.png",
                "kindle-logo-tall.png"
            ]
        }
    }

}
</script>

<style>

</style>