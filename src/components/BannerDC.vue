<script>
    export default {
        name: "BannerDC",
        data(){
            return {
                bannerLinks: [
                    {
                        name: "DIGITAL COMICS",
                        url: "#",
                        path: "buy-comics-digital-comics.png"
                    },
                    {
                        name: "DC MERCHANDISE",
                        url: "#",
                        path: "buy-comics-merchandise.png"
                    },
                    {
                        name: "SUBSCRIPTION",
                        url: "#",
                        path: "buy-comics-shop-locator.png"
                    },
                    {
                        name: "COMIC SHOP LOCATOR",
                        url: "#", 
                        path: "buy-comics-subscriptions.png"
                    },
                    {
                        name: "DC POWER VISA",
                        url: "#",
                        path: "buy-dc-power-visa.svg"
                    },
                ] 
            }
        }
    }
</script>

<template>
    <div class="outer">
        <nav>
            <ul>
              <li v-for="(object, index) in bannerLinks" :key="index">
                <img src="../assets/buy-comics-digital-comics.png" alt="link">
                <a :href="object.url">
                    {{object.name}}
                </a>
              </li>  
            </ul>
        </nav>
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
