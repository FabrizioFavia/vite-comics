<script>
export default {
    name: "AppJumbotron"
}
</script>


<template>
    <div class="jumboBox">
        <img class="jumbo" src="/assets/jumbotron.jpg" alt="">
    </div>
</template>

<style lang="scss">
@use "../main.scss" as *;


.jumboBox {
    max-height: 410px;

    .jumbo {
        max-height: 410px;
        width: 100%;
        object-fit: cover;
        object-position: top;
    }
}
</style>