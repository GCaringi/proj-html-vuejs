<template>
    <section id = "critics" class = "w-[var(--width-xxl)] m-auto py-[4rem]">
        <div class = "flex justify-between items-center">
            <section-header
                title = "What The Critics Say"
                subtitle = "Testimonials from around the world"
                class = "text-[color:var(--clr-secondary)]"
            />
            <btn-symbol
                elem = "Read All Testimonials"
                class="bg-[color:var(--clr-primary)] py-2 px-7 text-[color:var(--clr-base-light)] font-semibold rounded-md"
            />
        </div>
        <div>

        </div>
    </section>
</template>

<script>

import btnSymbol from '../atoms/a-btnSymbol.vue'
import sectionHeader from '../molecules/m-sectionsHeader.vue'

export default {
    name: "criticsSection",
    components: {
        btnSymbol,
        sectionHeader,
    }
}
</script>

<style>

</style>