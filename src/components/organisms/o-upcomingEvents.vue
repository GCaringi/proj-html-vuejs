<template>
  <section id = "upcoming" class = "bg-[color:var(--clr-bg-secondary)]">
        <div class = "w-[var(--width-xxl)] m-auto">
            <header-section
                title = "Upcoming Events"
                subtitle = "Meet the Autor in person"
                class= "text-center text-[color:var(--clr-primary)] py-[3rem]"
            />
            <div class = "flex gap-x-[3rem]">
                <classic-card
                    v-for = "(info, index) in infoCard"
                    :key = "index"
                    :title = "info.title"
                    :content= "info.content"
                    :src= "info.img"
                />
            </div>
        </div>
  </section>
</template>

<script>

import headerSection from '../molecules/m-sectionsHeader.vue'
import classicCard from '../molecules/m-classicCard.vue'

export default {
    name : "upComingEvents",
    components: {
        headerSection,
        classicCard,
    },
    data(){
        return {
            infoCard : [
                {
                    img: "event-05-400x240.jpg",
                    title: "Chicago Book Signing",
                    content: "Mauris bandit aliquet, eget tincidunt nibh pulvinar a Mauris blandit, aliquet elit eget tincidunt nibh pulvinar a nulla",
                },
                {
                    img: "event-04-400x240.jpg",
                    title: "Meet & Greet With Amanda",
                    content: "Mauris bandit aliquet, eget tincidunt nibh pulvinar a Mauris blandit, aliquet elit eget tincidunt nibh pulvinar a nulla",
                },
                {
                    img: "event-07-400x240.jpg",
                    title: "Open Book: Dialogues",
                    content: "Mauris bandit aliquet, eget tincidunt nibh pulvinar a Mauris blandit, aliquet elit eget tincidunt nibh pulvinar a nulla",
                }
            ]
        }
    }
}
</script>

<style>

</style>