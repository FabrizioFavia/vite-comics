<script>
export default {
    name: "AppMidNav",

    data() {
        return {
            icons: [
                {
                    img: "/assets/buy-comics-digital-comics.png",
                    dscrpt: "DIGITAL COMICS"
                },
                {
                    img: "/assets/buy-comics-merchandise.png",
                    dscrpt: "DC MERCHANDISE"
                },
                {
                    img: "/assets/buy-comics-subscriptions.png",
                    dscrpt: "SUBSCRIPTION"
                },
                {
                    img: "/assets/buy-comics-shop-locator.png",
                    dscrpt: "COMIC SHOP LOCATOR"
                },
                {
                    img: "/assets/buy-dc-power-visa.svg",
                    dscrpt: "DC POWER VISA",
                    width: "big"
                },
            ]
        }
    }
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