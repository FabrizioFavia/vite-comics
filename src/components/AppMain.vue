<script>
export default {
    name: "AppMain",
    props: ["comics"],
}
</script>


<template>
    <main>
        <div class="mainPart">
            <div class="container-lg p-5 d-flex justify-content-between flex-wrap">
                <template v-for="comic in comics">
                    <div class="comic">
                        <img class="comicImg" :src="comic.thumb" alt="">
                        <p class="mt-3 text-white">{{ comic.series.toUpperCase() }}</p>
                    </div>
                </template>
            </div>
        </div>
    </main>
</template>

<style lang="scss">
@use "../main.scss" as *;

.mainPart {
    width: 100%;
    max-height: 680px;
    background-color: $secondaryColor
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