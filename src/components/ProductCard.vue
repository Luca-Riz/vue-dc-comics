<template>
    <div class="product-card">
        <img :src="prod.src" :alt="prod.titolo">
    </div>
</template>

<script>
export default {
    name: 'ProductCard',
    props: ["prod", "testo", "titolo"]
}
</script>

<style>

</style>