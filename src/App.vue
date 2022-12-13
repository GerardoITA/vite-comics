<script>
import HeaderDC from './components/HeaderDC.vue'
import MainDC from './components/MainDC.vue'
import BannerDC from './components/BannerDC.vue'

export default {
  name: "App",
  components: {
    HeaderDC,
    MainDC,
    BannerDC,
  }
}
</script>

<template>
 <HeaderDC></HeaderDC>
 <MainDC></MainDC>
 <BannerDC></BannerDC>
</template>

<style lang="scss">
@use "./styles/partials/variables" as *;
@use "./styles/partials/mixins" as *;
@use "./styles/general.scss" as *;
</style>
