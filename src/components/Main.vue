<template>

    <main>
        <section class="contents">
            <div class="sizeContainer"></div>
        </section>
        <section class="merchandise">
            <div class="sizeContainer"></div>
        </section>
    </main>
  
</template>

<script>
// script
export default {
    name: "Main"
}
</script>

<style lang="scss" scoped>
    main {
        background-color: rgb(37, 37, 37);
        height: 300px;

        .contents {
            height: 150px;
        }
        .merchandise {
            height: 150px;
            background-color: #0282f9;

            .sizeContainer {
                background-color: rgba(255, 255, 255, 0.116);
                height: 100%;
            }
        }
    }
</style>