<script>
    export default {
        name: "BannerDC",
        data(){
            return {
                bannerLinks: [
                    {
                        name: "DIGITAL COMICS",
                        url: "#",
                        path: "../assets/buy-comics-digital-comics.png"
                    },
                    {
                        name: "DC MERCHANDISE",
                        url: "#",
                        path: "../assets/buy-comics-merchandise.png"
                    },
                    {
                        name: "SUBSCRIPTION",
                        url: "#",
                        path: "../assets/buy-comics-shop-locator.png"
                    },
                    {
                        name: "COMIC SHOP LOCATOR",
                        url: "#", 
                        path: "../assets/buy-comics-subscriptions.png"
                    },
                    {
                        name: "DC POWER VISA",
                        url: "#",
                        path: "../assets/buy-dc-power-visa.svg"
                    },
                ] 
            }
        },
        methods: {
        getImageURL: function (imgPath) {
            return new URL(imgPath, import.meta.url).href
        }
    }
    }
</script>

<template>
    <div class="outer">
        <div class="innerOuter">
            <nav>
                <ul>
                    <li v-for="(object, index) in bannerLinks" :key="index">
                        <img :src="getImageURL(object.path)" alt="link">
                        <a :href="object.url">
                            {{ object.name }}
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
        
    </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
    .outer {
        background-color: $DCblue;
    }
        nav {
            box-sizing: border-box;
    
            ul {
                display: flex;
                flex-wrap: nowrap;
    
                li {
                    list-style: none;
                    margin: 0 2rem 0;
                    display: flex;
                    justify-content: center;
                    align-items: center;
    
                    a {
                        display: inline-block;
                        padding: 3rem 0;
                        text-decoration: none;
                        color: white;
                        font-weight: 400;
                        margin: 2rem;
                        

                    }
    
                }
            }
        }
        img {
            height: 5rem;
            width: auto;

        }
</style>
