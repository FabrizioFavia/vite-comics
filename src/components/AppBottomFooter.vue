<script>
export default {
    name: "AppBottomFooter"
}
</script>


<template>
    <div class="bottomFooter d-flex justify-content-between align-items-center">
        <div class="container-lg d-flex justify-content-between align-items-center">
            <div class="leftPart">
                <button class="text-white px-3 py-2">SIGN-UP NOW!</button>
            </div>
            <div class="RightPart d-flex justify-content-between align-items-center">
                <h4 class="text-primary mt-2 me-3"><a href="">FOLLOW US</a></h4>
                <img class="ms-3" src="/assets/footer-facebook.png" alt="">
                <img class="ms-3" src="/assets/footer-twitter.png" alt="">
                <img class="ms-3" src="/assets/footer-youtube.png" alt="">
                <img class="ms-3" src="/assets/footer-pinterest.png" alt="">
                <img class="ms-3" src="/assets/footer-periscope.png" alt="">


            </div>
        </div>
    </div>
</template>

<style scoped>
.bottomFooter {
    width: 100%;
    height: 110px;
    background-color: #303030;
    z-index: 2;
    position: absolute;
}

button {
    background-color: #303030;
    border: 2px solid #0282f9;
    font-size: 20px;
}

button:hover {
    background-color: #0282f9;
}

h4>a {
    font-weight: bold;
    text-decoration: none;
}
</style>