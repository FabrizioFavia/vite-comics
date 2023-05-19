<script>
export default {
    name: "AppMidNav",

    data() {
        return {
            icons: [
                {
                    img: "../assets/jumbotron.jpg"
                }
            ]
        }
    }
}
</script>


<template>
    <div class="midNav d-flex justify-content-center">

        <div v-for="icon in icons" class="container-lg d-flex align-items-center border border-dark">
            <img :src="icon.img" alt="">
        </div>
    </div>
</template>

<style scoped>
.midNav {
    width: 100%;
    height: 155px;
    /* background-color: #0282f9; */
}
</style>