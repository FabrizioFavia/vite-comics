<script>
export default {
    name: "AppMidNav",
    props: ["icons"]
}
</script>


<template>
    <div class="midNav d-flex justify-content-center">

        <div v-for="icon in icons" class="imgbox d-flex align-items-center justify-content-center">
            <img :class="icon.dscrpt == `DC POWER VISA` ? `imgCustom` : ` img`" :src="icon.img" alt="icon"
                class="white-text">
            <a class="text-white" href="">{{ icon.dscrpt }}</a>
        </div>
    </div>
</template>

<style lang="scss">
@use "../main.scss" as *;

.midNav {
    width: 100%;
    height: 155px;
    background-color: $primaryColor;
    position: relative;
    z-index: 4;
}

.imgbox {
    width: 270px;
    color: white;
    font-size: 16px;
}

.imgcontainer {
    color: white;
    font-size: 16px;
}

.img {
    height: 55px;
    padding-right: 20px;
}

.imgCustom {
    height: 40px;
    padding-right: 20px;
}

a {
    text-decoration: none;
}
</style>