<template>
  <div>
    <large-text
        :text = "title"
        class = "text-[color:var(--clr-base-dark)] text-[2rem]"
    />
    <sub-title
        :text = subtitle
        class = "text-[1.125rem]"
    />
  </div>
</template>

<script>

import largeText from '../atoms/a-largeText.vue'
import subTitle from '../atoms/a-subTitles.vue'

export default {
    name: "sectionHeader",
    components: {
        largeText,
        subTitle,
    },
    props: {
        title: {
            type: String,
        },
        subtitle: {
            type: String,
        }
    }
}
</script>

<style>

</style>