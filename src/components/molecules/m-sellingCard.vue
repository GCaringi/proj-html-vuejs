<template>
  <div class = "flex flex-col bg-[color:var(--clr-base-light)] w-[30%] absolute bottom-0 right-0 p-6" >
    <div class = "flex">
        <image-page
            source = "book-widget.png"
        />
        <div class="flex flex-col pt-4 pr-6">
            <littleTitle
                text = "Latest book Relase"
                class="pt-5"
            />
            <sub-titles
                text = "D. Vaughn Autobiography"
                class = "text-[color:var(--clr-primary)] py-4 text-sm"
            />
            <medium-text
                text = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus sint ratione magni expedita officia inventore"
            />
        </div>
    </div>
    <div class = "shadow-[0px_0px_10px_10px_#F5FCFA]">
        <button class = "w-1/2 border border-[color:var(--clr-secondary)] bg-[#F5FCFA]  border-r-0 py-2 text-xs"><i class="fa-brands fa-amazon"></i> Buy on Amazon</button>
        <button class = "w-1/2 border border-[color:var(--clr-secondary)] bg-[#F5FCFA] py-2 text-xs"><i class="fa-brands fa-apple"></i> Buy on AppStore</button>
    </div>
  </div>
</template>

<script>

import imagePage from '../atoms/a-imagePage.vue'
import littleTitle from '../atoms/a-littleTitle.vue'
import subTitles from '../atoms/a-subTitles.vue'
import mediumText from '../atoms/a-mediumText.vue'

export default {
    name: "sellingCard",
    components: {
        imagePage,
        littleTitle,
        subTitles,
        mediumText,
    }
}
</script>

<style lang = "scss" scoped>

</style>