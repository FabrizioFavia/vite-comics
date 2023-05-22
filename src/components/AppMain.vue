<script>
export default {
    name: "AppMain",
    props: ["comics"]
}
</script>


<template>
    <main>
        <div class="mainPart">
            <div class="container-lg p-5 d-flex justify-content-between flex-wrap">
                <template v-for="comic in comics">
                    <div class="comic">
                        <img class="comicImg" :src="comic.thumb" alt="">
                        <h3>{{ comic.series }}</h3>
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
    width: 190px;
    height: 240px;
    border: 1px solid white;
    margin-top: 3em;
    margin-left: 1em;
}
</style>