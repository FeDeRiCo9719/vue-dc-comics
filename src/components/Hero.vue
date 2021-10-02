<template>
    <!-- HERO -->
    <section class="hero" :style="`background-image: url(${imgBg})`">
        <div class="sizeContainer">
            <div>CURRENT SERIES</div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Hero",
    props: ['imgBg'],
}
</script>
    
<style lang="scss" scoped>
    .hero {
        width: 100%;
        height: 500px;
        // background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;

        .sizeContainer {
            height: 500px;
            position: relative;

            div {
                position: absolute;
                bottom: -30px;
                left: 0px;

                padding: 10px 40px ;
                background-color: #0282f9;
                color: white;
                border: 1px solid #0282f9;     
                font-size: 30px;
                font-weight: 700;
            }
        }
    }
</style>