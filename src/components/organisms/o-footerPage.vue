<template>
    <header class="relative pt-[3rem]">
        <div class = "w-[var(--width-xxl)] m-auto p-[4rem] flex justify-between">
            <footer-text
                title= "About"
                content= " Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis tempore qui nobis aut deleniti expedita voluptatem sed perspiciatis. Totam id aut quisquam natus. A temporibus, quas molestias vitae ex praesentium?"
                class = "w-[30%] text-[color:var(--clr-typo-secondary)]"
            />
            <footer-list
                class = "w-[30%]"
            />
            <footer-contacts
                class="w-[30%] flex flex-col text-[color:var(--clr-typo-secondary)]"
            />
        </div>
            <div class="w-[var(--width-xxl)] m-auto text-center text-xs text-[color:var(--clr-typo-secondary)]">
                &copy; Copyright 2012-2020 | Avada Theme by <span class="text-white">ThemeFusion</span> | All Rights Reserved | Powered by <span class = "text-white" >Wordpress</span>
            </div>
        <image-page
            source= "author-logo-round-small.png"
            class = "absolute top-[30%] left-8"
        />
        <btn-symbol
            elem = "⋀"
            class= " absolute bottom-0 right-5  py-2 px-7 text-[color:var(--clr-base-light)] bg-zinc-800 rounded-md"
        />
    </header>
</template>

<script>

import footerText from '../molecules/m-footerText.vue'
import footerList from '../molecules/m-footerList.vue'
import footerContacts from "../molecules/m-footerContacts.vue"
import imagePage from '../atoms/a-imagePage.vue'
import btnSymbol from '../atoms/a-btnSymbol.vue'


export default {
    name: "footerPage",
    components: {
        footerText,
        footerList,
        footerContacts,
        imagePage,
        btnSymbol,
    }
}
</script>

<style lang = "scss" scoped>

header{
    background-image: url("@/assets/img/hero-07-2x.jpg"), linear-gradient(0deg, rgba(0,0,0,0.8) 30%, rgba(255,255,255,0) 100%);
    background-blend-mode: color;
    background-size: cover;
}

</style>