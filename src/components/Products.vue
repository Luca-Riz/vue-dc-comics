<template>
    <div class="all-width">
        <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="">
        </div>
        <div class="container products">

            <div class="current">Current series</div>

            <div class="products-area">
                <!-- passo i dati a ProductCard -->
                <ProductCard  v-for="(prod,index) in products"
                :key="index"
                :prod="prod" /> 
            </div>

            <div class="load-more">Load more</div>
            
        </div>
    </div>

</template>

<script>

import ProductCard from './ProductCard.vue';
import ProdItems from '@/data/ProdItems.js';

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
        text-align: center;

        img{
            max-width: 100%;
            height: auto;
        }
    }

    .products {
        height: 100%;
        position: relative;
        text-align: center;

        .current {
            color: white;
            text-transform: uppercase;
            background-color: $blue-dc;
            display: inline-block;
            padding: 0.75rem 1rem;
            font-size: 1.5rem;
            font-weight: 500;
            position: absolute;
            top: calc(-3rem / 2);
            left: 0;
            cursor: pointer;
        }

        .products-area{
            display: flex;
            flex-wrap: wrap;
        }

        .load-more {
            color: white;
            text-transform: uppercase;
            background-color: $blue-dc;
            display: inline-block;
            padding: 0.5rem 5rem;
            font-weight: 500;
            cursor: pointer;
            margin-bottom: 1rem;    
        }
        
    }
}


</style>