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
                    dscrpt: "SUBSCRIPTIONS"
                },
                {
                    img: "/assets/buy-comics-shop-locator.png",
                    dscrpt: "COMIC SHOP LOCATOR"
                },
                {
                    img: "/assets/buy-dc-power-visa.svg",
                    dscrpt: "DC POWER VISA"
                },
            ]
        }
    }
}
</script>


<template>
    <div class="midNav d-flex justify-content-center">

        <div v-for="icon in icons" class="imgbox d-flex align-items-center justify-content-center">
            <div class="imgcontainer d-flex align-items-center">
                <img :src="icon.img" alt="icon" class="white-text"> {{ icon.dscrpt }}
            </div>

        </div>
    </div>
</template>

<style scoped>
.midNav {
    width: 100%;
    height: 155px;
    background-color: #0282f9;
}

.imgbox {
    width: 270px;
    justify-content: flex-start;
}

.imgcontainer {
    color: white;
}

img {
    height: 50px;
    padding-right: 20px;
}
</style>