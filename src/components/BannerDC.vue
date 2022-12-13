<script>
    export default {
        name: "BannerDC",
        data(){
            return {
                
            }
        }
    }
</script>

<template>
    <div class="outer">
        <h1>--> Content goes here &lt-- </h1>
    </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
    .outer {
        background-color: $DCblue;
    }
    h1 {
        color: white;
    }
</style>
