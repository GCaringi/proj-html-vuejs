<template>
    <div class = "m-bigCard flex flex-col w-1/2 text-[color:var(--clr-base-light)] p-[4rem] leading-relaxed rounded-br-[12%]">
        <large-text
            text = "Best Author of His Generation"
            class= "pt-[2.5rem] text-[2.5rem] pb-4"
        />
        <hr class = "w-full m-auto pb-8">
        <medium-text
            text = "This book will change your prospective on life"
            class= "font-semibold "
        />
        <medium-text
            text = "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vero qui sunt, nostrum nulla saepe, illo exercitationem placeat reiciendis doloribus accusamus, numquam inventore deserunt ducimus delectusnumquam inventore deserunt"
            class = "py-5 "
        />

        <medium-text
            text = "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vero qui sunt, nostrum nulla saepe, illo exercitationem placeat reiciendis doloribus accusamus, numquam inventore deserunt ducimus delectus voluptates. Impedit fugiat voluptate dolor?  "
            class= "pb-5"
        />
        <div class = "flex items-center font-bold pb-[2.5rem]">
            <image-page
                source= "nytimes-logo-white-xsmall.png"
                class= "pr-3"
            />
            <little-text
                text = "Justine Kilpatrick,"
                class= "text-sm"
            />
            <little-text
                text = "The New York Times"
                class="text-sm text-[color:var(--clr-secondary)]"
            />
        </div>
    </div>
</template>

<script>

import imagePage from '../atoms/a-imagePage.vue'
import largeText from '../atoms/a-largeText.vue'
import mediumText from '../atoms/a-mediumText.vue'
import littleText from '../atoms/a-littleText.vue'

export default {
    name: "bigCard",
    components: {
        largeText,
        mediumText,
        imagePage,
        littleText,
    }
}
</script>

<style lang = "scss" scoped>

.m-bigCard{
    background-image: url("@/assets/img/testimonial2-2x.jpg"), linear-gradient(0deg, rgba(0,0,0,0.8) 30%, rgba(255,255,255,0) 100%);
    background-blend-mode: color;
    background-size: cover;
    background-position: center;
}

</style>