<template>
    <header>
    <div class="container">
        <a href="#">
            <img src="./../assets/img/dc-logo.png" alt="">
        </a>
        <nav>
            <ul>
                <li v-for="(link, index) in links" key="index">
                    <div class="link" :class="{'active': link.current }">
                        <a :href="link.url" @click="sceltaPagina(index)">{{link.text}}</a>
                        
                    </div>
                    <div class="linea" :class="{'active': link.current }"></div>
                </li>
            </ul>
        </nav>
    </div>
        
    </header>
</template>

<script>

    export default {
        name:'HeaderComponent',
        data() {
            return {
                links: [
                    {
                        text: "characters",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "comics",
                        url: "#",
                        current: true,
                    },
                    {
                        text: "movies",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "tv",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "games",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "collectibles",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "videos",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "fans",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "news",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "shop",
                        url: "#",
                        current: false,
                    }

                ]
            }
        },
        methods:{
                
        }
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;
    // @use '../assets/styles/general.scss' as *;

    header{
        overflow-x: hidden;
        background-color: $white;
        .container{
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        ul{
            display: flex;
            justify-content: flex-end;


            li{
                height: 100%;
                
                div.link{
                    padding: 10px;
                    
                    a{
                        
                        text-transform: uppercase;
                        color: $black;
                    }
                    
                }
                div.linea{
                    // background-color: $blue;
                    height: 5px;
                    position: relative;
                    top: 30px;
                }
                .link.active a{
                    color: $blue;
                }
                .linea.active{
                    background-color: $blue;
                }
            }
        }
    }
</style>