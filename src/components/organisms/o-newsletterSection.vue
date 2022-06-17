<template>
  <section id = "newsletter">
        <div class = "w-[var(--width-md)] m-auto flex flex-col justify-center text-center py-[6rem]">
            <large-text
                text = "Subscribe To My"
                class="text-5xl pb-2"
            />
            <large-text
                text= "Newsletter"
                class="text-5xl"
            />
            <sub-title
                text = "be notified about signing tour dates"
                class="text-[color:var(--clr-primary)] tracking-widest"
            />
            <form class = "flex justify-center gap-x-4 pt-8">
                <input type="email" name="" id="" placeholder="Insert your email ...*" class = "w-[40%] rounded-md p-3">
                <btn-symbol
                    elem = "Subscribe"
                    class="w-[25%] bg-[color:var(--clr-secondary)] text-[color:var(--clr-base-light)] px-8 py-3 rounded-md font-bold" 
                />
            </form>
            <little-text
                text = "Lorem ipsum, dolor sit amet consectetur adipisicing elit."
                class = "text-[color:var(--clr-sponsors)] pt-8 font-semibold"
            />
        </div>
  </section>
</template>

<script>


import largeText from '../atoms/a-largeText.vue'
import subTitle from '../atoms/a-subTitles.vue'
import littleText from '../atoms/a-littleText.vue'
import btnSymbol from '../atoms/a-btnSymbol.vue'

export default {
    name: "newsletterSection",
    components: { 
        largeText,
        subTitle,
        littleText,
        btnSymbol,
    }
}
</script>

<style lang = "scss" scoped>

#newsletter{
    background-image: url("@/assets/img/banner-2.jpg"), linear-gradient(0deg, rgba(0,0,0,0.8) 30%, rgba(255,255,255,0) 100%);
    background-blend-mode: color;;
    background-size: cover;
}


</style>