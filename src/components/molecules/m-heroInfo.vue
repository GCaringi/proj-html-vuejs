<template>
  <div class = "w-1/2 py-12">
    <big-title
        text = "Damon Vaugh"
        class = "text-6xl pt-5"
    />
    <large-text
        text = "Best-selling author and most influential public intellectual in the western world right now"
        class = "text-[2.5rem] text-[var(--clr-base-light)] py-5"
    />
    <little-text
        text = " - The New York Times"
        class="text-[1rem] text-[color:var(--clr-typo-secondary)]"
    />
    <div class="flex pt-8 gap-x-1">
        <btn-symbol
            elem = "←"
            class = "bg-black text-white font-bold text-xl px-3 py-2 rounded-md"
        />
        <btn-symbol
            elem = "→" 
            class= "bg-black text-white font-bold text-xl px-3 py-2 rounded-md"
        />
    </div>
  </div>
</template>

<script>

import bigTitle from '../atoms/a-bigTitle.vue'
import largeText from '../atoms/a-largeText.vue'
import littleText from '../atoms/a-littleText.vue'
import btnSymbol from '../atoms/a-btnSymbol.vue'

export default {
    name: "heroInfo",
    components: {
        bigTitle,
        largeText,
        littleText,
        btnSymbol,
    }
}
</script>

<style>

</style>