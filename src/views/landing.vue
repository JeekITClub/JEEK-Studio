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
            <div class="title">
                用心做产品，用脚做设计
            </div>
            <div class="desc">
                每个人都是产品经理
            </div>
            <div class="cards row">
                <product-card class="col-md-3 mr-auto ml-auto" title="123" desc="ads" :url="url1">
                </product-card>
                <product-card class="col-md-3 mr-auto ml-auto" title="123" desc="ads" :url="url1">
                </product-card>
                <product-card class="col-md-3 mr-auto ml-auto" title="123" desc="ads" :url="url1">
                </product-card>
            </div>
        </div>
        <div class="container members">
            <div class="title">
                奇怪的人写奇怪的代码
            </div>
            <div class="desc">
                竟然还有一个不是学计算机的
            </div>
            <div class="subdesc">
                一帮奇怪的计算机爱好者组成的工作室。他们来自不同的学校，不同的专业，甚至有一位不是计算机专业的。
            </div>
            <div class="cards row">
                <member-card
                    class="col-md-3 mr-auto ml-auto"
                    :url="url1"
                    name="Cheney Ni" 
                    desc="东方霍格沃斯">
                </member-card>
                <member-card
                    class="col-md-3 mr-auto ml-auto"
                    :url="url1"
                    name="Harvey Ni" 
                    desc="法学的东方明珠">
                </member-card>
                <member-card
                    class="col-md-3 mr-auto ml-auto"
                    :url="url1"
                    name="Artanic Qiu" 
                    desc="东方膜法学院">
                </member-card>
            </div>
        </div>
        <div class="container plans">
            <div class="title">
            </div>
            <div class="desc">
            </div>
            <div class="row plans">
                <plan-card class="col-md-2" :price="233"></plan-card>
            </div>
        </div>
    </div>
    
</template>

<script>
import ProductCard from '../components/product'
import MemberCard from '../components/member'
import PlanCard from '../components/plan'
export default {
    components: {
        ProductCard,
        MemberCard,
        PlanCard
    },
    data () {
        return {
            url1: require('../assets/product.jpg')
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
        margin-bottom: 10vh;
        border-radius: 1vh;
        padding-top: 2vh;
        padding-bottom: 10vh;
        box-shadow: -1px 2px 14px 1px #888888;
        .title {
            text-align: center;
            font-size: 2.4rem;
        }
        .desc {
            margin-top: 1vh;
            text-align: center;
            font-size: 1.2rem;
        }
        .cards {
            margin-top: 3vh;
        }
    }
    .members {
        box-shadow: 2px -1px 14px 1px #888888;
        padding-top: 2vh;
        border-radius: 1vh;
        .title {
            margin-left: 5vh;
            font-size: 2.4rem;
        }
        .desc {
            margin-top: 1vh;
            margin-left: 8vh;
            font-size: 1.2rem;
        }
        .subdesc {
            margin-top: 5vh;
            margin-left: 8vh;
            font-size: 1rem;
        }
        .cards {
            margin-top: 3vh;
        }
    }
    .plans {
        margin: 5vh;
    }
</style>
