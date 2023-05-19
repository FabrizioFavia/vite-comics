<script>
export default {
    name: "AppHeader"
}
</script>


<template>
    <header>
        <div class="container-lg d-flex align-items-center">
            <div class="navbar w-100 d-flex justify-content-between align-items-center">
                <div class="logoContainer">
                    <img class="headerLogo" src="/assets/dc-logo.png" alt="">
                </div>
                <div class="navItems d-flex align-items-center">
                    <div class="item">CHARACTERS</div>
                    <div class="item">COMICS</div>
                    <div class="item">MOVIES</div>
                    <div class="item">TV</div>
                    <div class="item">GAMES</div>
                    <div class="item">COLLECTIBLES</div>
                    <div class="item">VIDEOS</div>
                    <div class="item">FANS</div>
                    <div class="item">NEWS</div>
                    <div class="item">SHOP</div>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
header {
    width: 100%;
    height: 115px;
}

.container-lg {
    height: 100%;
}

.headerLogo {
    height: 75px;
}

.navItems {
    height: 115px;
    line-height: 110px;
}

div.item {
    margin: 0 10px;
    height: 115px;
    font-size: 12px;
    font-weight: bold;
}

.item:hover {
    color: #0282f9;
    border-bottom: 4px solid #0282f9;

}
</style>