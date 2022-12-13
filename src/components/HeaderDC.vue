<script>
    export default {
        name: "HeaderDC",
        data(){
            return {
                links: [
                {   url: "#",
                    text: "CHARACTERS",
                    current: false,
                },
                {   url: "#",
                    text: "COMICS",
                    current: true,
                },
                {   url: "#",
                    text: "MOVIES",
                    current: false,
                },
                {   url: "#",
                    text: "TV",
                    current: false,
                },
                {   url: "#",
                    text: "GAMES",
                    current: false,
                },
                {   url: "#",
                    text: "COLLECTIBLES",
                    current: false,
                },
                {   url: "#",
                    text: "VIDEOS",
                    current: false,
                },
                {   url: "#",
                    text: "FANS",
                    current: false,
                },
                {   url: "#",
                    text: "NEWS",
                    current: false,
                },
                {   url: "#",
                    text: "SHOP",
                    current: false,
                },
                ]
            }
        }
    }
</script>

<template>
    <div class="outer">
        <div class="outerInner">
            <a href="/" class="logoDC">
                <img src="../assets/dc-logo.png" alt="Logo DC">
            </a>
            
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a :href="link.url" :class="{ active: link.current }">
                            {{ link.text }}
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
        background-color: white;
        
    }
    nav {
        box-sizing: border-box;
        ul {
                display: flex;
        
                li {
                    list-style: none;
                    margin: 0 2rem 0;
                    a {
                        display: inline-block;
                        padding: 3rem 0;
                        text-decoration: none;
                        color: $DCgrey;
                        font-weight: 600;
                       
        
                        &:active,
                        &:hover {
                            color: $DCblue;
                            border-bottom: 6px solid $DCblue;
                        }
                    }
        
                }
            }
    }
</style>
