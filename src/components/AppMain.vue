<script>
export default {
    name: "AppMain",
    props: ["comics"],
}
</script>


<template>
    <main>
        <div class="mainPart">

            <div class="container-lg p-5">
                <div class="currentS text-white p-2 d-flex justify-content-center">
                    CURRENT SERIES
                </div>
                <div class="comicContainer d-flex justify-content-between flex-wrap">
                    <template v-for="comic in comics">
                        <div class="comic">
                            <img class="comicImg" :src="comic.thumb" alt="">
                            <p class="mt-3 text-white">{{ comic.series.toUpperCase() }}</p>
                        </div>
                    </template>
                </div>
                <div class="d-flex justify-content-center">
                    <button class="label text-white mt-5 px-5">LOAD MORE</button>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss">
@use "../main.scss" as *;

.mainPart {
    width: 100%;
    min-height: 680px;
    background-color: $secondaryColor;
    position: relative;
}

.currentS {
    width: 250px;
    background-color: $primaryColor;
    position: absolute;
    top: -30px;
    font-size: 28px;
    font-weight: bold;
}

.label {
    background-color: $primaryColor;
}
</style>

<style scoped>
.comic {
    width: 180px;
    height: 240px;
    margin-top: 2em;
    margin-left: 1em;
}

.comicImg {
    width: 100%;
    height: 190px;
    object-fit: cover;
    object-position: top;
}
</style>