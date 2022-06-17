<template>
   <div class = "flex items-center pb-[2.5rem]">
            <image-page
                :source= "src"
                class= "pr-3"
            />
            <little-text
                :text = "author"
                class= "text-sm font-bold"
            />
            <little-text
                :text = "journal"
                class="text-sm"
            />
    </div>
</template>


<script>

import imagePage from './a-imagePage.vue'
import littleText from './a-littleText.vue'

export default {
    name: "authorCitation",
    components:{
        imagePage,
        littleText,
    },
    props: {
        src : {
            type:String,
        },
        author: {
            type:String,
        },
        journal: {
            type:String,
        }
    }
}
</script>

<style>

</style>