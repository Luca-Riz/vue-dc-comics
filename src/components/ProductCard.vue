<template>
    <div class="product-card">
        <div class="img-div">
            <img :src="prod.thumb" :alt="prod.series">
        </div>
        <div class="titolo-card"> {{ prod.series }} </div>
    </div>
</template>

<script>
    export default {
    name: 'ProductCard',
    props: ["prod"]
    }
</script>

<style lang="scss" scoped>

    .product-card {
        width: calc(100% / 12 * 2);
        padding: 3rem 1rem;

        .img-div {
            height: 200px;
            overflow: hidden;
        }

        .titolo-card {
            color:white;
            text-transform: uppercase;
            padding-top: 1rem;
            text-align: left;
        }
    }



</style>