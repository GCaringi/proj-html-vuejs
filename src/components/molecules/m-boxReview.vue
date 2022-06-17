<template>
  <div class = "flex flex-col items-center justify-center bg-[color:var(--clr-bg-secondary)] text-center ">
    <little-title
        :text = "title"
        class= "text-xl font-semibold"
    />
    <medium-text
        :text= "content"
        class= "text-sm leading-relaxed text-[color:var(--clr-sponsors)] py-4 px-[3rem]"
    />
  </div>
</template>

<script>

import littleTitle from '../atoms/a-littleTitle.vue'
import mediumText from '../atoms/a-mediumText.vue'

export default {
    name: "boxReview",
    components: {
        littleTitle,
        mediumText,
    },
    props: {
        title: {
            type: String,
        },
        content: {
            type: String,
        },
    }
}
</script>

<style>

</style>