<template>

    <footer>
        <!-- top footer  -->
        <section class="topFooter">
            <div class="sizeContainer">
                <div>
                    <div class="links_box">
                        <h2>DC COMICS</h2>
                        <ul>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Comics</a>
                            </li>
                            <li>
                                <a href="#">Movies</a>
                            </li>
                            <li>
                                <a href="#">TV</a>
                            </li>
                            <li>
                                <a href="#">Games</a>
                            </li>
                            <li>
                                <a href="#">Videos</a>
                            </li>
                            <li>
                                <a href="#">News</a>
                            </li>
                        </ul>
                    </div>

                    <div class="links_box">
                        <h2>SHOP</h2>
                        <ul>
                            <li>
                                <a href="#">Schop DC</a>
                            </li>
                            <li>
                                <a href="#">Schop DC Collectibles</a>
                            </li>
                        </ul>
                    </div>

                </div>
                
                <div class="links_box">
                    <h2>DC</h2>
                    <ul>
                        <li>
                            <a href="#">Terms Of Use</a>
                        </li>
                        <li>
                            <a href="#">Privacy Policy(News)</a>
                        </li>
                        <li>
                            <a href="#">Add Choices</a>
                        </li>
                        <li>
                            <a href="#">Advertising</a>
                        </li>
                        <li>
                            <a href="#">Job</a>
                        </li>
                        <li>
                            <a href="#">Subscriptions</a>
                        </li>
                        <li>
                            <a href="#">Talent Workshops</a>
                        </li>
                        <li>
                            <a href="#">CPSC Certificates</a>
                        </li>
                        <li>
                            <a href="#">Ratings</a>
                        </li>
                        <li>
                            <a href="#">Shop Help</a>
                        </li>
                        <li>
                            <a href="#">Contact Us</a>
                        </li>
                    </ul>
                </div>

                <div class="links_box">
                    <h2>SITES</h2>
                    <ul>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="#">DC Kids</a>
                        </li>
                        <li>
                            <a href="#">DC Universe</a>
                        </li>
                        <li>
                            <a href="#">DC Power Visa</a>
                        </li>
                    </ul>
                </div>
                
            </div>
        </section>
        <section class="lowFooter">
            <div class="sizeContainer">
                <div>
                    <button>SIGN-UP NOW!</button>
                </div>
                <div class="follow">
                    <h3>FOLLOW US</h3>
                    <ul class="social_links">
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-facebook.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-twitter.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-youtube.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-pinterest.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/footer-periscope.png" alt="">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </section>
    </footer>
  
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style lang="scss" scoped>
    footer {
        .topFooter {
            background-image: url('../assets/img/footer-bg.jpg');
            background-repeat: no-repeat;
            background-position: center top;
            background-size: cover;
            position: relative;

            .sizeContainer {
                background-image: url('../assets/img/dc-logo-bg.png');
                background-position: right center;
                background-repeat: no-repeat;
                height: 100%;
                padding: 40px 0px;

                display: flex;

                .links_box {
                    margin-right: 30px;
                    margin-bottom: 15px;
                    cursor: pointer;

                    a {
                        color: grey;
                        font-size: 14px;
                    }
                    a:hover {
                        color: #0282f9;
                    }

                    h2 {
                        color: white;
                        font-size: 20px;
                        margin-bottom: 10px;
                    }
                }
            }
        }
        .lowFooter {
            background-color: rgb(53, 53, 53);
            height: 120px;

            .sizeContainer {
                height: 100%;
                display: flex;
                justify-content: space-between;
                align-items: center;

                button {
                    padding: 15px;
                    border: 2px solid #0282f9;
                    background-color: rgba(0, 0, 0, 0);
                    color: white;
                    font-size: 16px;
                    cursor: pointer;
                }
                button:hover {
                    transition: 0.2s;
                    background-color: #0282f9;
                }

                .follow {
                    height: 100%;
                    display: flex;
                    align-items: center;
                    
                    h3 {
                        color: #0282f9;
                        font-size: 22px;
                    }

                    .social_links {
                        display: flex;

                        li {
                            margin-left: 20px;
                        }
                    }

                }
            }
        }
    }
</style>