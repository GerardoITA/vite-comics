<script>
    export default {
        name: "FooterDC",
        data(){
            return {
                DCComics: [
                    {
                        name: "Characters",
                        url: "#"
                    },
                    {
                        name: "Comics",
                        url: "#"
                    },
                    {
                        name: "Movies",
                        url: "#"
                    },
                    {
                        name: "TV",
                        url: "#"
                    },
                    {
                        name: "Games",
                        url: "#"
                    },
                    {
                        name: "Videos",
                        url: "#"
                    },
                    {
                        name: "News",
                        url: "#"
                    },


                ],
                DC: [
                    {
                        name: "Terms of Use",
                        url: "#"
                    },
                    {
                        name: "Privacy policy (New)",
                        url: "#"
                    },
                    {
                        name: "Ad Choices",
                        url: "#"
                    },
                    {
                        name: "Advertising",
                        url: "#"
                    },
                    {
                        name: "Jobs",
                        url: "#"
                    },
                    {
                        name: "Subscriptions",
                        url: "#"
                    },
                    {
                        name: "Talent Workshops",
                        url: "#"
                    },
                    {
                        name: "CSPS Certificates",
                        url: "#"
                    },
                    {
                        name: "Ratings",
                        url: "#"
                    },
                    {
                        name: "Show Help",
                        url: "#"
                    },
                    {
                        name: "Contact Us",
                        url: "#"
                    },


                ],
                Sites: [
                    {
                        name: "DC",
                        url: "#"
                    },
                    {
                        name: "MAD Magazine",
                        url: "#"
                    },
                    {
                        name: "DC Kids",
                        url: "#"
                    },
                    {
                        name: "DC Universe",
                        url: "#"
                    },
                    {
                        name: "DC Power Visa",
                        url: "#"
                    },
                ],
                Shop: [
                    {
                        name: "Shop DC",
                        url: "#"
                    },
                    {
                        name: "Shop DC Collectibles",
                        url: "#"
                    },
                
                ],
            }
        }
    }
</script>

<template>
    <div class="outer">
        <div class="outerInner">
            <nav>
                <ul>
                    <h4>DC COMICS</h4>
                    <li v-for="(link, index) in DCComics" :key="index">
                        <a :href="link.url">
                            {{link.name}}
                        </a>
                    </li>
                </ul>
                <ul>
                    <h4>DC</h4>
                    <li v-for="(link, index) in DC" :key="index">
                        <a :href="link.url">
                            {{link.name}}
                        </a>
                    </li>
                </ul>
                <ul>
                    <h4>SHOP</h4>
                    <li v-for="(link, index) in Sites" :key="index">
                        <a :href="link.url">
                            {{link.name}}
                        </a>
                    </li>
                </ul>
                <ul>
                    <h4>SHOP</h4>
                    <li v-for="(link, index) in Shop" :key="index">
                        <a :href="link.url">
                            {{link.name}}
                        </a>
                    </li>
                </ul>
            </nav>
            <img src="../assets/dc-logo-bg.png" alt="">
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
        height: 23rem;
    }
    .outerInner {
        overflow: hidden;
    }
    img {
        height: 35rem;
        width: auto;
    }
    h4 {
        color: white;
        margin-bottom: 1rem;
    }
    nav {
        box-sizing: border-box;
        min-height: 18rem;
        width: 500px;
        display: flex;
        flex-wrap: wrap;

        ul {
            display: flex;
            flex-direction: column;
            justify-content: flex-start;

            li {
                list-style: none;
                margin: 1px;

                a {
                     display: inline-block;
                    text-decoration: none;
                    color: rgb(180, 180, 180);
                    font-weight: 400; 
                    &:hover {
                        color: rgb(225, 225, 225);
                    }

                }

            }
        }
    }
</style>
