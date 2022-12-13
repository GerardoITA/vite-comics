<script>
    export default {
        name: "LinkFooterDC",
        data(){
            return {
                footerLinks: [
                    {
                        path: "../assets/footer-facebook.png",
                        url: "#"
                    },  
                    {
                        path: "../assets/footer-periscope.png",
                        url: "#"
                    },
                    {
                        path: "../assets/footer-pinterest.png",
                        url: "#"
                    },
                    {
                        path: "../assets/footer-twitter.png",
                        url: "#"
                    },
                    {
                        path: "../assets/footer-youtube.png",
                        url: "#"
                    }
                ]
            }
        },
        methods: {
            getImageURL: function (imgPath){
                return new URL(imgPath, import.meta.url).href
            }
        }
    }
</script>

<template>
    <div class="outer">
        <div class="outerInner">
            <button>SIGN UP NOW!</button>
            <div class="linkBar">
                <div class="linkBarText">
                    FOLLOW US
                </div>
                <ul>
                    <li v-for="(link, index) in footerLinks" :key="index">
                        <a :href="link.url"><img :src="getImageURL(link.path)" alt="."></a>
                    </li>
                </ul>
            </div>
        </div>
        
    </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
    .outer {
        background-color: $DClightgrey;
        min-height: 7rem;
    }
    button {
        background-color: $DClightgrey;
        border: 2px solid $DCblue;
        border-radius: 0;
        padding: 1rem;
        font-weight: 600;
        color: white;
        
        &:hover {
            cursor: pointer;

        }
    }
    .linkBar {
        display: flex;
        align-items: center;
        .linkBarText {
            font-weight: 600;
            color: $DCblue;
        }
        ul {
            display: flex;
            li {
                list-style: none;
                margin: 0 0.5rem 0;
            }
        }
    }
</style>
