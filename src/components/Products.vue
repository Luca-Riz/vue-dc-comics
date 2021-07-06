<template>
    <div class="all-width">
        <div class="container products">

            Content goes here
        </div>
    </div>

</template>

<script>
export default {
    name: 'Header',

    // data() {}
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.all-width {
    background-color: black;
    height: $std-height;
}

.products {
    height: 100%;
    color: white;
    display: flex;
    align-items: center;
}

</style>