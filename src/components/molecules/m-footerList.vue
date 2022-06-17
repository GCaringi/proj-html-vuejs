<template>
  <div>
    <little-title
        text= "Useful Link"
        class="text-[color:var(--clr-base-light)] uppercase pb-8 font-bold text-xl"
    />
    <ul>
        <nav-item
            v-for = "(link, index) in links"
            :key = "index"
            :text="link"
            class = "text-[color:var(--clr-base-light)] pb-3"
        />
    </ul>
  </div>
</template>

<script>

import littleTitle from '../atoms/a-littleTitle.vue'
import navItem from '../atoms/a-navItem.vue'

export default {
    name: "footerList",
    components: {
        littleTitle,
        navItem,
    },
    data() {
        return {
            links : [
                "Latest Book",
                "Upcoming Event",
                "Recent Articles",
                "Buisiness Enquires",
                "Visit My Foundation"
            ] 
        }
    }
}
</script>

<style lang = "scss" scoped>

li::before{
    content: "\f054";
    font-family: "Font Awesome 6 Free";
    font-weight: 900;
    padding-right: .5rem;
}


</style>