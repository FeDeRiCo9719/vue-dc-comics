<template>

    <header>
        <div class="sizeContainer">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="Logo Dc">
            </div>
            <nav>
                <ul>
                    <li v-for="(item, index) in menu" :key="index" >
                        <a :href="item.url" v-bind:class="item.current==true?'active':''">{{ item.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
  
</template>

<script>
export default {
    name: "Header",
    data() {
        return {
            menu: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: "true",
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: "false",
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: "false",
                },
                {
                    text: "TV",
                    url: "#",
                    current: "false",
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: "false",
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: "false",
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: "false",
                },
                {
                    text: "FANS",
                    url: "#",
                    current: "false",
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: "false",
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: "false",
                },

            ]
        }
    } 
}
</script>

<style lang="scss" scoped>
// @import './variables';
    header {
        height: 120px;

        .sizeContainer {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;

            .logo {
                height: 70%;
                img {
                    height: 100%;
                }               
            }

            nav ul {
                display: flex;
                align-items: center;

                li {
                    margin-left: 40px;
                    
                    a {
                        color: rgb(70, 70, 70);
                        font-weight: 700;

                        &.active {
                            color: #0282f9;
                        }
                    }
                    
                }
            }
        }
    }
</style>