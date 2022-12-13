<script>
    export default {
        name: "JumbotronDC",
        data(){
            return {
            
            }
        }
    }
</script>

<template>
    <div class="outer">

    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
    .outer {
        background-image: url(../assets/jumbotron.jpg);
        background-size:cover;
        background-color: $DClightgrey;
        height: 30rem;
    }
</style>
