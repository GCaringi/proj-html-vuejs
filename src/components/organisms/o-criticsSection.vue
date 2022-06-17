<template>
    <section id = "critics" class = "w-[var(--width-xxl)] m-auto py-[4rem]">
        <div class = "flex justify-between items-center pb-4">
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
        <div class = "flex pt-4 items-start">
            <big-card
                class = "w-[55%]"
            />
            <div class = "w-[45%] flex flex-col pl-[6rem] justify-between">
                <box-review
                    :title = "reviews[0].title"
                    :content= "reviews[0].content"
                    class=" p-[2rem] "
                /> 
                <author-citation
                    :src = "reviews[0].src"
                    :author= "reviews[0].author"
                    :journal= "reviews[0].journal"
                    class="pt-4"
                />
                <box-review
                    :title = "reviews[1].title"
                    :content= "reviews[1].content"
                    class=" p-[2rem]"
                />
                <author-citation
                    :src = "reviews[1].src"
                    :author= "reviews[1].author"
                    :journal= "reviews[1].journal"
                    class = "pt-4"
                />
            </div>
        </div>
    </section>
    
</template>

<script>

import btnSymbol from '../atoms/a-btnSymbol.vue'
import sectionHeader from '../molecules/m-sectionsHeader.vue'
import bigCard from '../molecules/m-bigCard.vue'
import boxReview from '../molecules/m-boxReview.vue'
import authorCitation from '../atoms/a-authorCitations.vue'

export default {
    name: "criticsSection",
    components: {
        btnSymbol,
        sectionHeader,
        bigCard,
        boxReview,
        authorCitation,
    },
    data(){
        return {
            reviews: [
                {
                    title: "A true Masterpiece, Bravo!",
                    content: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum aspernatur necessitatibus veniam consectetur aperiam harum optio fuga voluptate unde exercitationem at velit reiciendis, aliquam eum repudiandae tempore atque magnam inventore.",
                    src: "theguardian-xsmall.png",
                    author: "Gearal Hendley,",
                    journal: "The Guardian"
                },
                {
                    title: "A Unique View On the World",
                    content: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum aspernatur necessitatibus veniam consectetur aperiam harum optio fuga voluptate unde exercitationem at velit reiciendis, aliquam eum repudiandae tempore atque magnam inventore.Lorem ipsum dolor sit amet consectetur adipisicing elit. ",
                    src: "globe-xsmall.png",
                    author: "Mary Maxey,",
                    journal: "The Globe and Mail"
                }
            ]
        }
    }
}
</script>

<style>

</style>