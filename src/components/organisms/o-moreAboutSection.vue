<template>
  <section id = "moreAbout" class = "w-[var(--width-xxl)] m-auto pb-[6rem]">
    <div class = "flex justify-center items-center text-center py-[3rem]">
        <section-header
            title = "Dig A Little Deeper Into Damon Vaughn"
            subtitle= "find out more about the author himself"
            class="text-[color:var(--clr-secondary)] font-bold" 
        />
    </div>
    <div class = "flex gap-x-12 ">
        <card-rounded
            v-for = "(info, index) in cardsInfo"
            :key = index
            :src="info.img"
            :title="info.title"
            :subt="info.subt"
            class="overflow-hidden rounded-br-[12%]"
        />
    </div>
  </section>
</template>

<script>

import sectionHeader from '../molecules/m-sectionsHeader.vue'
import cardRounded from '../molecules/m-cardRounded.vue'

export default {
    name: "moreAboutSection",
    components: {
        sectionHeader,
        cardRounded,
    },
    data(){
        return {
            cardsInfo: [
                {
                    img: "box-1.jpg",
                    title: "About me",
                    subt: "Vestibulum ante ipsum primis",
                },
                {
                    img: "box-4.jpg",
                    title: "My Latest Book",
                    subt: "Vestibulum ante ipsum primis",

                },
                {
                    img: "box-3.jpg",
                    title: "BookSigning",
                    subt: "Vestibulum ante ipsum primis",

                }
            ]
        }
    }
}
</script>

<style>

</style>