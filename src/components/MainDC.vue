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
            <div class="mainButton">
                CURRENT SERIES
            </div>
            <Slide v-for="slide in slides"
            :img="slide.thumb"
            :prezzo="slide.price"
            :serie="slide.series"
            :tipo="slide.type">
            </Slide> 
            <div class="smallButton">
                LOAD MORE
            </div>
            
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
        padding-top: 10rem;
        padding-bottom: 10rem;
        gap: 3rem;
        flex-wrap: wrap;
        position: relative;
    }
    .mainButton {
        padding: 1rem;
        font-size: 20px;
        color: white;
        background-color: $DCblue;
        position: absolute;
        top: -1.5rem;
        cursor: pointer;
    }
    .smallButton {
        padding: 1rem 3rem;
        font-size: 15px;
        color: white;
        background-color: $DCblue;
        position: absolute;
        bottom: 2rem;
        left: 50%;
        transform: translateX(-50%);
        cursor: pointer;
    }
</style>
