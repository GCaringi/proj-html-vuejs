<template>
  <section id = "recentArticles" class="bg-[color:var(--clr-bg-secondary)] py-[6rem]">
    <div class = "w-[var(--width-xxl)] m-auto"> 
        <div class = "flex justify-between items-center pb-4">
            <section-header
                title = "Recent Articles"
                subtitle = "Read the last entries"
                class = "text-[color:var(--clr-secondary)]"
            />
            <btn-symbol
                elem = "All Articles"
                class="bg-[color:var(--clr-primary)] py-2 px-7 text-[color:var(--clr-base-light)] font-semibold rounded-md"
            />
        </div>
        <div class = "flex gap-x-10">
            <box-article
                class="w-[65%] flex flex-col bg-[color:var(--clr-base-light)] p-8"
            />
            <div class="w-[30%] flex flex-col">
                <box-article-thumb
                    v-for = "(thumb, index) in thumbs"
                    :key = "index"
                    :src = "thumb.img"
                    :title = "thumb.title"
                    :sub = "thumb.small"
                    class="bg-[color:var(--clr-base-light)] h-full p-8 "
                />
            </div>
        </div>
    </div>
  </section>
</template>

<script>

import sectionHeader from '../molecules/m-sectionsHeader.vue'
import boxArticle from '../molecules/m-boxArticle.vue'
import boxArticleThumb from '../molecules/m-boxArticleThumb.vue'
import btnSymbol from '../atoms/a-btnSymbol.vue'

export default {
    name: "recentArticles",
    components: {
        sectionHeader,
        btnSymbol,
        boxArticle,
        boxArticleThumb,
    },
    data(){
        return {
            thumbs : [
                {
                    img : "thumb-13-2x-320x202.jpg",
                    title: "What's On Your Booklist?",
                    small: "October 24th, 2019 | 0 Comments",
                },
                {
                    img : "thumb-08-2x-320x202.jpg",
                    title: "Istanbul Travel Guide",
                    small: "October 24th, 2019 | 0 Comments",
                },
                
            ]
        }
    }
}
</script>

<style>

</style>