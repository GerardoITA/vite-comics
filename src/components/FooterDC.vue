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
        <div class="outerInner">
            <nav>
                <ul>

                </ul>
            </nav>
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
        nav {
            box-sizing: border-box;
    
            ul {
                display: flex;
    
                li {
                    list-style: none;
                    margin: 0 1rem 0;
    
                    a {
                        /* display: inline-block;
                        padding: 3rem 0;
                        text-decoration: none;
                        color: $DCgrey;
                        font-weight: 600; */
    

                    }
    
                }
            }
        }
</style>
