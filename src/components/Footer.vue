<template>

    <footer>
        <section class="upFooter">
            <div class="sizeContainer">
                <div class="links_box"></div>
                <div class="big_logo"></div>
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
                                <img src="@/assets/img/footer-facebook.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="@/assets/img/footer-twitter.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="@/assets/img/footer-youtube.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="@/assets/img/footer-pinterest.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="@/assets/img/footer-periscope.png" alt="">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </section>
    </footer>
  
</template>

<script>
// script
export default {
    name: "Footer"
}
</script>

<style lang="scss" scoped>
    footer {
        .upFooter {
            background-image: url('../assets/img/footer-bg.jpg');
            background-position: center top;
            background-repeat: no-repeat;
            background-size: cover;
            height: 350px;

            .sizeContainer {
                display: flex;
                justify-content: space-between;
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