<template>
  <div>
    <image-page
      :source= "src"
      class="w-full pb-4 "
    />
    <little-title
      :text= "title"
      class = "text-xl tracking-widest"
    />
    <little-text
      :text= "sub"
    />
  </div>
</template>

<script>

import imagePage from '../atoms/a-imagePage.vue'
import littleTitle from '../atoms/a-littleTitle.vue'
import littleText from '../atoms/a-littleText.vue'

export default {
    name: "boxArticleThumb",
    components: {
      imagePage,
      littleTitle,
      littleText,
    }, props: {
            src: {
              type:String,
            },
            title: {
              type:String,
            },
            sub: {
              type:String,
            }

    }
}
</script>

<style>

</style>