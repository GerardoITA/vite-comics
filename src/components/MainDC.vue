<script>
    import json from "../assets/dc-comics.json"
    import Slide from "../components/main/SlidesDC.vue"
    
    export default {
        name: "MainDC",
        components: {
            Slide
        },
        data(){
            return {
                slides: json
            }
        }
    }
</script>

<template>
    <div class="outer">
        <div class="outerInner">
            <Slide v-for="slide in slides"
            :img="slide.thumb"
            :prezzo="slide.price"
            :serie="slide.series"
            :tipo="slide.type">
            </Slide> 

            
        </div>
        
    </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
    .outer {
        background-color: $DCgrey;
        min-height: calc(100vh - 50rem)
    }
    .outerInner {
        justify-content: flex-start;
        align-items: center;
        gap: 3rem;
        flex-wrap: wrap;
    }
</style>
