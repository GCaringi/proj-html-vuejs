<template>
    <nav class= "pt-8 relative">
        <ul class = "list-none flex text-white gap-x-8">
            <nav-item
                v-for = "(link, index) in navLinks"
                :key = "index"
                :text = "link"
                class = "a-navItem relative font-semibold"
            />
            <li>
                <i class="fa-solid fa-cart-shopping"></i>
            </li>
        </ul>
    </nav>
</template>

<script>

import navItem from '../atoms/a-navItem.vue'

export default {
    name: "navBar",
    data(){
        return {
            navLinks : ["Home", "About me", "Testimonials", "My blog", "Meetups", "Shop", "Contact Me"],
        }
    },
    components: {
        navItem,
    }
}

</script>

<style lang = "scss" scoped >

li:hover{
    color: var(--clr-primary);
}

.a-navItem:hover::before{
    content: "";
    width: 100%;
    height: .3125rem;
    background-color: var(--clr-primary);
    position: absolute;
    top: -2rem;
}

.active{
    color: var(--clr-primary)
}


</style>