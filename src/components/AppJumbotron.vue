<script>
export default {
    name: "AppJumbotron"
}
</script>


<template>
    <div class="jumboBox">
        <img src="/assets/jumbotron.jpg" alt="">
    </div>
</template>

<style lang="scss">
@use "../main.scss" as *;

main {
    width: 100%;
    min-height: 130px;
    background-color: #222;
}

.jumboBox {
    max-height: 300px;

    img {
        max-height: 300px;
        width: 100%;
        object-fit: cover;
        object-position: top;
    }
}
</style>