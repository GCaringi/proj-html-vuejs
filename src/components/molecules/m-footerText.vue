<template>
  <div>
    <little-title
        :text= "title"
        class="text-[color:var(--clr-base-light)] uppercase pb-8 font-bold text-xl"
    />
    <little-text
        :text= "content"
    />
  </div>
</template>

<script>

import littleTitle from '../atoms/a-littleTitle.vue'
import littleText from '../atoms/a-littleText.vue'

export default {
    name: "footerText",
    components: {
        littleTitle,
        littleText,
    },
    props: {
        content: {
            type:String,
        },
        title: {
            type: String,
        }
    }
}
</script>

<style>

</style>