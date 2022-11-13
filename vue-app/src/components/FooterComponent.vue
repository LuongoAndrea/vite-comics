<template>
    <footer>
        <section class="bg-blue ">
            <div class="d-flex container">
                <div class="card">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <span>comics digital</span>
                </div>
                <div class="card">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <span>comics digital</span>
                </div>
                <div class="card">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <span>comics digital</span>
                </div>
                <div class="card">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <span>comics digital</span>
                </div>
                <div class="card">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <span>comics digital</span>
                </div>
            </div>
        </section>
        <section class="ul">
            <div class="container d-flex">
                <div class="li">
                    <div>
                        <ul><h2>dc comics</h2>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                        </ul>
                        
                            <ul><h2>shop</h2>
                            <li>character</li>
                            <li>character</li>
                        </ul>
                        
                        
                    </div>
                    <div>
                        <ul><h2>dc</h2>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                        </ul>
                    </div>
                    <div>
                        <ul><h2>sites</h2>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                            <li>character</li>
                        </ul>
                    </div>
                </div>
                <div class="img">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
            
        </section>
        <section class="info">
        <div class="container">
            <div>
                <button>sing up now!</button>
            </div>
            <div>
                <div><span><a href="#">follow us</a></span></div>
                
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">
            </div>
        </div>
        </section>
    </footer>
</template>

<script>
    export default {
        name:'FooterComponent'
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;
    section.bg-blue{
        background-color: $blue;
        padding: 20px;
    }
    span{
        text-transform: uppercase;
        color: $white;
    }
    .d-flex{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    img{
        width: 20%;
        
    }
    .card{
        display: flex;
        align-items: center;
        justify-content: space-around;
        width: calc((100%) / 5);
        
    }
    section.ul{
        display: flex;
        justify-content: space-around;
        overflow: hidden;
        background-image: url(../assets/img/footer-bg.jpg);
        div.container.d-flex{
            ul{
                text-transform: uppercase;
            }
            li{
                text-transform: capitalize;
            }
            div.img{
                height: 50px;
                position: relative;
                img{
                    width: 80%;
                    position: relative;
                    top: -200px;
                    right: -80px;
                }
            }
            
        }
        h2{
            padding: 20px 0;
            color: $white;
        }
        div.li{
            display: flex;
            color: $li;
            div{
                margin: 0 20px;
            }
        }
    
    }
    section.info{
        background-color: $grey;
       div.container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        div{
            display: flex;
            align-items: center;
            justify-content: space-between;
            button{
                padding: 10px;
                text-transform: uppercase;
                background-color: $grey;
                color: $white;
                border: 3px solid $blue;
            }
            div{
                width: 10rem;
            }
            span a{
                color: $blue;
            }
        }
       }
    }

</style>