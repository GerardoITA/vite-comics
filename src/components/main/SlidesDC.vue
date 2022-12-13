<script>
    export default {
        name: "SlidesDC",
        props :{
            img: String,
            prezzo: String,
            serie: String,
            tipo: String,
        }
    }
</script>

<template>
    <div class="slide">

    </div>

</template>

<style lang="scss" scoped>
    h3 {
        margin-top: 1rem;
        color: white;
    }
</style>

            :img="slide.thumb"
            :prezzo="slide.price"
            :series="slide.series"
            :tipo="slide.type">