<template>

    <main>
        <!-- COMICS -->
        <section class="contents">
            <div class="sizeContainer">
                <!-- items -->
                <div class="boxComics">
                    <div>a</div>
                    <div>a</div>
                    <div>a</div>
                    <div>a</div>
                    <div>a</div>
                    <div>a</div>
                    <div>a</div>
                    <div>a</div>
                    <div>a</div>
                    <div>a</div>
                </div>

                <!-- button -->
                <div>
                    <button>LOAD MORE</button>
                </div>

            </div>
        </section>

        <!-- INFO -->
        <section class="info">
            <div class="sizeContainer">
                <ul>
                    <li v-for="(item, index) in info" :key="index">
                        <a href="#">
                            <img :src="item.img" alt="INFO img">
                            <div>{{ item.name }}</div>
                        </a>
                    </li>
                </ul>
            </div>
        </section>
    </main>
  
</template>

<script>
export default {
    name: "Comics",
    data() {
        return {
            info: [
                {
                    name: "DIGITAL COMICS",
                    img: require("../assets/img/buy-comics-digital-comics.png"),
                },
                {
                    name: "DC MERCHANDISE",
                    img: require("../assets/img/buy-comics-merchandise.png"),
                },
                {
                    name: "SUBSCRIPTION",
                    img: require("../assets/img/buy-comics-subscriptions.png"),
                },
                {
                    name: "COMIC SHOP LOCATOR",
                    img: require("../assets/img/buy-comics-shop-locator.png"),
                },{
                    name: "DC POWER VISA",
                    img: require("../assets/img/buy-comics-digital-comics.png"),
                }
            ],
            series: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
    main {
        background-color: rgb(37, 37, 37);

        .contents {
            padding: 20px;
            padding-top: 50px;

            .sizeContainer {
                display: flex;
                flex-direction: column;
                align-items: center;
                gap: 40px;
            }

            .boxComics {
                display: flex;
                justify-content: center;
                flex-wrap: wrap;
                gap: 10px;

                div {
                    width: 250px;
                    height: 250px;
                    background-color: red;
                }
            }

            button {
                padding: 10px 60px;
                background-color: #0282f9;
                color: white;
                border: 1px solid #0282f9;     
                font-size: 12px;
                font-weight: 700;
                cursor: pointer;
            }
        }
        .info {
            height: 200px;
            background-color: #0282f9;

            .sizeContainer {
                // background-color: rgba(236, 58, 58, 0.445);
                height: 200px;

                ul {
                    height: 200px;
                    display: flex;
                    align-items: center;
                    justify-content: space-around;
                }

                a {
                    // background-color: rgba(171, 238, 14, 0.486);
                    color: white;
                    display: flex;
                    align-items: center;
                    gap: 10px;

                    img {
                        width: 50px;
                    }
                }
            }
        }
    }
</style>