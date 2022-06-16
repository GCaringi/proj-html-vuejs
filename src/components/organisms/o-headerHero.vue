<template>
  <div class = "section__wrapper bg-cover bg-center relative">
    <header-page/>
    <hero-main/>
    <selling-card/>
    <demos-btn/>
    <price-sale/>
  </div> 
</template>

<script>

import headerPage from '../organisms/o-headerPage.vue'
import heroMain from '../organisms/o-heroMain.vue'
import sellingCard from '../molecules/m-sellingCard.vue'
import demosBtn from '../particles/p-demosBtn.vue'
import priceSale from '../particles/p-priceSale.vue'

export default {
  name: "headerHero",
  components: {
    headerPage,
    heroMain,
    sellingCard,
    demosBtn,
    priceSale,
  }
}
</script>

<style lang = "scss" scoped>

.section__wrapper{
    background-image: url("@/assets/img/hero-07-2x.jpg"), linear-gradient(0deg, rgba(0,0,0,0.8) 30%, rgba(255,255,255,0) 100%);
    background-blend-mode: color;
}

</style>