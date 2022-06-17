<template>
  <div>
    <image-page
        source="20-Tips-600x353.jpg"
        class="w-full pb-8"
    />
    <little-title
        text = "20 Creativity Tips"
        class="text-2xl pb-2 tracking-widest"
    />
    <little-text
        text = "By Admin | October 24th, 2019 | Categories: Event, Tips and Tricks"
        class="pb-4"
    />
    <little-text
        text = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus nostrum natus voluptates. Quisquam nobis mollitia voluptatum, laudantium consequatur rem tenetur libero, dolor sit amet consectetur adipisicing elit. Accusamus nostrum natus voluptates. "
        class="pb-4 pr-4"
    />
  </div>
  
</template>

<script>

import imagePage from '../atoms/a-imagePage.vue'
import littleTitle from '../atoms/a-littleTitle.vue'
import littleText from '../atoms/a-littleText.vue'

export default {
    name: "boxArticle",
    components: {
        imagePage,
        littleTitle,
        littleText,
    },

}
</script>

<style>

</style>