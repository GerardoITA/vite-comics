<script>
    import json from "../assets/dc-comics.json"
    export default {
        name: "MainDC",
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
            <h1>-->  </h1>
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
    h1 {
        color: white;
    }
</style>
