<template>
  <div>
    <little-title
        text="Contact Info"
        class = "text-[color:var(--clr-base-light)] uppercase pb-8 font-bold text-xl"
    />
    <little-text
        v-for = "(row, index) in info"
        :key = "index"
        :text= "row"
        class = "pb-4"
    />
    <div class = "flex gap-x-4 pt-3 text-[color:var(--clr-typo-secondary)]">
        <i class="fa-brands fa-facebook"></i>
        <i class="fa-brands fa-twitter"></i>
        <i class="fa-brands fa-instagram"></i>
        <i class="fa-brands fa-linkedin-in"></i>
        <i class="fa-brands fa-youtube"></i>
    </div>
  </div>
</template>

<script>

import littleTitle from "../atoms/a-littleTitle.vue"
import littleText from "../atoms/a-littleText.vue"

export default {
    name: "footerContacts",
    components: {
        littleTitle,
        littleText
    },
    data(){
        return {
            info: [
                "63 E. Studabaker Street BolingBrook, IL 60440",
                "Phone: (800) 000 - 0000",
                "Mobile: (800) 000 - 0000",
                "Email: info@your-company.com"
            ]
        }
    }
}
</script>

<style>

</style>