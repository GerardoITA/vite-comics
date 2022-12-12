<script>
import HeaderDC from './components/HeaderDC.vue'

export default {
  name: "App",
  components: {
    HeaderDC
  }
}
</script>

<template>
 <HeaderDC></HeaderDC>
</template>

<style lang="scss">
@use "./styles/partials/variables" as *;
@use "./styles/partials/mixins" as *;
@use "./styles/general.scss" as *;
</style>
