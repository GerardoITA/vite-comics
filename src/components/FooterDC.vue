<script>
    export default {
        name: "FooterDC",
        data(){
            return {
                
            }
        }
    }
</script>

<template>
    <div class="outer">
        <div class="inner">
            
        </div>
    </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
    .outer {
        background-image: url(../assets/footer-bg.jpg);
        background-size:cover;
        background-color: $DClightgrey;
        min-height: 23rem;
    }
    .inner {
        width: 100%;
        height: fit-content;
        
    }
    h1 {
        color: white;
    }
</style>
