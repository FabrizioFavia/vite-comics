<script>
import AppBottomFooter from '../components/AppBottomFooter.vue'
export default {
    name: "AppFooter",
    components: {
        AppBottomFooter
    }

}
</script>


<template>
    <div class="topFooter">
        <div class="container-lg">
            <div class="row justify-content-evenly">
                <div class="col-6">
                    <div class="row pt-5">
                        <div class="col-3">
                            <p class="text-white title fs-4">DC COMICS</p>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Comics</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">TV</a></li>
                                <li><a href="#">Games</a></li>
                                <li><a href="#">Videos</a></li>
                                <li><a href="#">News</a></li>
                            </ul>

                            <p class="text-white title fs-4">SHOP</p>
                            <ul>
                                <li><a href="#">Shop DC</a></li>
                                <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </div>
                        <div class="col-3">
                            <p class="text-white title fs-4">DC</p>
                            <ul>
                                <li><a href="#">Terms Of Use</a></li>
                                <li><a href="#">Privacy policy (New)</a></li>
                                <li><a href="#">Ad Choices</a></li>
                                <li><a href="#">Advertising</a></li>
                                <li><a href="#">Jobs</a></li>
                                <li><a href="#">Subscriptions</a></li>
                                <li><a href="#">CPSC Certificates</a></li>
                                <li><a href="#">Ratings</a></li>
                                <li><a href="#">Shop Help</a></li>
                                <li><a href="#">Contact Us</a></li>
                            </ul>
                        </div>
                        <div class="col-3">
                            <p class="text-white title fs-4">SITES</p>
                            <ul>
                                <li><a href="#">DC</a></li>
                                <li><a href="#">MAD Magazine</a></li>
                                <li><a href="#">DC kids</a></li>
                                <li><a href="#">DC Universe</a></li>
                                <li><a href="#">DC Power Visa</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-6 logoContainer">
                    <img src="/assets/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
    </div>
    <AppBottomFooter />
</template>

<style scoped>
.topFooter {
    width: 100%;
    height: 459px;
    background-image: url("/assets/footer-bg.jpg");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
}

.col5 {
    min-height: 100%;
}

.title {
    font-weight: bold;
}

.logoContainer {

    padding-bottom: 100px;
    position: relative;

}

img {
    width: 103%;
    position: absolute;
    top: -29%;
    z-index: 1;
    opacity: 80%;
}

ul {
    list-style-type: none;
    padding-left: 0;
}

li {
    font-size: 14px;
    color: rgb(140, 141, 137);
    margin-bottom: 3px;
}

a:hover {
    color: white;
}

li>a {
    text-decoration: none;
    color: rgb(140, 141, 137);
}

.bottomFooter {
    width: 100%;
    height: 110px;
    background-color: #303030;
    z-index: 2;
    position: absolute;
}
</style>

