<template>
  <div class = "w-[var(--width-xl)] m-auto display flex flex-col py-[6rem] items-center text-center">
    <big-title
        text = "More about Damon Vaugn"
        class = "text-6xl pb-8"
    />
    <medium-text
        text = "Damon Vaughn is a professor of psychology at the University of Toronto, a clinical psychologist
                and the author of the multi-million copv bestseller 'The story of my life'"
        class = "text-lg px-5 pb-8"
    />
    <btn-symbol
        elem = "Meet The Autor"
        class = "bg-[color:var(--clr-secondary)] rounded-md px-4 py-1 text-[color:var(--clr-base-light)] font-semibold"
    />
  </div>
</template>

<script>

import bigTitle from '../atoms/a-bigTitle.vue'
import mediumText from '../atoms/a-mediumText.vue'
import btnSymbol from '../atoms/a-btnSymbol.vue'

export default {
    name: "aboutInfo",
    components: {
        bigTitle,
        mediumText,
        btnSymbol,
    }
}
</script>

<style>

</style>