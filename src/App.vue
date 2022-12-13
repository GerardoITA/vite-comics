<script>
import HeaderDC from './components/HeaderDC.vue'
import MainDC from './components/MainDC.vue'
import BannerDC from './components/BannerDC.vue'
import FooterDC from './components/FooterDC.vue'
import LinkFooterDC from './components/LinkFooterDC.vue'
import JumbotronDC from './components/JumbotronDC.vue'

export default {
  name: "App",
  components: {
    HeaderDC,
    MainDC,
    BannerDC,
    FooterDC,
    LinkFooterDC,
    JumbotronDC,
  }
}
</script>

<template>
 <HeaderDC></HeaderDC>
 <JumbotronDC></JumbotronDC>
 <MainDC></MainDC>
 <BannerDC></BannerDC>
 <FooterDC></FooterDC>
 <LinkFooterDC></LinkFooterDC>
</template>

<style lang="scss">
@use "./styles/partials/variables" as *;
@use "./styles/partials/mixins" as *;
@use "./styles/general.scss" as *;
</style>
