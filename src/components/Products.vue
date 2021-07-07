<template>
    <div class="all-width">
        <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="">
        </div>
        <div class="container products">

            <div class="current">Current series</div>

            <div class="products-area">
                <!-- inserisco richiamo -->
                <ProductCard 
                
                /> 
            </div>

            <div class="load-more">Load more</div>
            
        </div>
    </div>

</template>

<script>
export default {
    name: 'Products',
    components: {
        ProductCard
    },
    data(){
        return {
            products: ProdItems,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/vars.scss';

.all-width {
    background-color: black;

    .jumbotron {
        height: 400px;
        overflow: hidden;
        img{
            max-width: 100%;
            height: auto;
        }
    }

    .products {
        height: 100%;

        .current {
            color: white;
        }
        
    }
}


</style>