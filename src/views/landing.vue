<template>
    <div>
        <div class="landing-pic">
            <div class="container">
                <div class="row" style="padding-bottom: 10vh;">
                    <div class="col col-md-8 ml-auto mr-auto">
                        <div class="brand">
                            <h1 class="brand-title">JEEK</h1>
                            <div class="brand-desc">
                                KEEP HACKING
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="container products">
            <div class="products-title">
                用心做产品，用脚做设计
            </div>
            <div class="products-desc">
                每个人都是产品经理
            </div>
            <product-card></product-card>
        </div>
    </div>
    
</template>

<script>
import ProductCard from '../components/product'
export default {
    components: {
        ProductCard
    },
    data () {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>
    .landing-pic {
        height: 90vh;
        background-image: url('../assets/landing.jpg');
        display: flex;
        align-items: center;
    }
    .brand {
        text-align: center;
        .brand-title {
            font-size: 7rem;
        }
        .brand-desc {
            font-size: 2rem;
        }
    }
    .products {
        margin-top: -5vh;
        background-color: white;
        min-height: 50vh;
        border-top-left-radius: 1vh;
        border-top-right-radius: 1vh;
        padding-top: 2vh;
        padding-bottom: 1vh;
        .products-title {
            text-align: center;
            font-size: 2.4rem;
        }
        .products-desc {
            margin-top: 1vh;
            text-align: center;
            font-size: 1.2rem;
        }
    }
</style>
