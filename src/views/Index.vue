<template>
    <div id="app">
        <div class="page-container">
            <div class="fullpage-wp" v-fullpage="opts" ref="main">
                <div class="page-1 page">
                    <b-button-group class="guide">
                            <b-button class="menuList1" >首页</b-button>
                            <b-button @click="moveNext" class="menuList1" >主要业务介绍</b-button>
                            <b-button @click="moveNext2" class="menuList1">主要作品</b-button>
                            <b-button @click="moveNext3" class="menuList1">人员介绍</b-button>
                            <b-button @click="moveNext4" class="menuList1">主要联系方式</b-button>
                    </b-button-group>
                    <div class="page-content">
                        <h1 class="main-title" v-animate="{value: 'bounceInLeft'}">Jeek Studio</h1>
                    </div>
                </div>
                <div class="page-4 page">
                     <b-button-group class="guide">
                            <b-button @click="movePrev" class="menuList4">首页</b-button>
                            <b-button  class="menuList4" >主要业务介绍</b-button>
                            <b-button @click="moveNext" class="menuList4">主要作品</b-button>
                            <b-button @click="moveNext2" class="menuList4">人员介绍</b-button>
                            <b-button @click="moveNext3" class="menuList4">主要联系方式</b-button>
                     </b-button-group>
                    <h1 class="title" v-animate="{value: 'bounceInLeft', delay: 0}">网站开发</h1>
                    <v-web  class="part-4" v-animate="{value: 'bounceInLeft', delay: 600}"></v-web>
                    <v-web2 class="part-4" v-animate="{value: 'bounceInRight', delay: 1200}"></v-web2>
                    <v-web3 class="part-4" v-animate="{value: 'zoomInDown', delay: 1600}"></v-web3>
                </div>
                 <div class="page-4 page">
                     <b-button-group class="guide">
                            <b-button @click="movePrev" class="menuList4">首页</b-button>
                            <b-button  class="menuList4">主要业务介绍</b-button>
                            <b-button @click="moveNext" class="menuList4">主要作品</b-button>
                            <b-button @click="moveNext2" class="menuList4">人员介绍</b-button>
                            <b-button @click="moveNext3" class="menuList4">主要联系方式</b-button>
                     </b-button-group>
                    <h1 class="title" v-animate="{value: 'bounceInLeft', delay: 0}">微信开发</h1>
                    <v-wechat class="part-4" v-animate="{value: 'bounceInRight', delay: 600}"></v-wechat>
                    <v-wechat2 class="part-4" v-animate="{value: 'bounceInRight', delay: 1200}"></v-wechat2>
                      <v-wechat3 class="part-4" v-animate="{value: 'zoomInDown', delay: 1600}"></v-wechat3>
                </div>
                <div class="page-3 page">
                    <b-button-group class="guide">
                            <b-button @click="movePrev2" class="menuList3">首页</b-button>
                            <b-button @click="movePrev" class="menuList3" >主要业务介绍</b-button>
                            <b-button  class="menuList3" >主要作品</b-button>
                            <b-button @click="moveNext" class="menuList3">人员介绍</b-button>
                            <b-button @click="moveNext2" class="menuList3">主要联系方式</b-button>
                    </b-button-group>
                     <h1 class="title" v-animate="{value: 'bounceInLeft', delay: 600}">主要作品</h1>
                    <v-pro class="part-3" v-animate="{value: 'pulse', delay: 1200}"></v-pro>
                </div>
                <div class="page-3 page">
                    <b-button-group class="guide">
                            <b-button @click="movePrev2" class="menuList3">首页</b-button>
                            <b-button @click="movePrev" class="menuList3" >主要业务介绍</b-button>
                            <b-button  class="menuList3" >主要作品</b-button>
                            <b-button @click="moveNext" class="menuList3">人员介绍</b-button>
                            <b-button @click="moveNext2" class="menuList3">主要联系方式</b-button>
                    </b-button-group>
                     <h1 class="title" v-animate="{value: 'bounceInLeft', delay: 600}">主要作品</h1>
                    <v-pro2 class="part-32" v-animate="{value: 'pulse', delay: 1200}"></v-pro2>
                    <p  color="white" v-animate="{value: 'zoomInDown', delay: 1600}">context context context</p>
                </div>
                <div class="page-2 page">
                        <b-button-group class="guide">
                            <b-button @click="movePrev3" class="menuList2">首页</b-button>
                            <b-button @click="movePrev2" class="menuList2" >主要业务介绍</b-button>
                            <b-button @click="movePrev" class="menuList2">主要作品</b-button>
                            <b-button class="menuList2" >人员介绍</b-button>
                            <b-button @click="moveNext" class="menuList2">主要联系方式</b-button>
                        </b-button-group>
                        <v-member1  class="part-2" v-animate="{value: 'bounceInLeft', delay: 1200}"></v-member1>
                        <v-member2  class="part-2" v-animate="{value: 'zoomInDown', delay: 0}"></v-member2>
                        <v-member3  class="part-2" v-animate="{value: 'bounceInRight', delay: 600}"></v-member3>

                </div>
                 <div class="page-5 page">
                     <b-button-group class="guide">
                            <b-button @click="movePrev4" class="menuList5">首页</b-button>
                            <b-button @click="movePrev3" class="menuList5" >主要业务介绍</b-button>
                            <b-button @click="movePrev2" class="menuList5">主要作品</b-button>
                            <b-button @click="movePrev" class="menuList5">人员介绍</b-button>
                            <b-button class="menuList5" >主要联系方式</b-button>
                     </b-button-group>
                     <h2>If you have questions, are looking for assistance or<br> just want to share your feedback with us, we're listening.</h2>
                    <v-con class="part-5" v-animate="{value: 'bounceInLeft', delay: 400}">fullpage-vue</v-con>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import WTO from "../components/Members/WTO"
    import NI from "../components/Members/NI"
    import pdd from "../components/Members/PDD"
    import website from "../components/Website/Website"
    import website2 from "../components/Website/Website2"
    import website3 from "../components/Website/Website3"
    import wechat from "../components/Wechat/Wechat"
    import wechat2 from "../components/Wechat/Wechat2"
    import wechat3 from "../components/Wechat/Wechat3"
    import pro from "../components/Product/Product"
    import pro2 from "../components/Product/Product2"
    import con from "../components/Contact"
    export default {
        name: 'Index',
        data() {
            return {
                opts: {
                    start: 0,
                    dir: 'v',
                    duration: 500,
                    beforeChange: function (prev, next) {
                        console.log(prev, next);
                    },
                    afterChange: function (prev, next) {
                        console.log(prev, next);
                    }
                }
            }
        },
        methods: {    //todo rebuild function(move)
            movePrev() {
                this.$refs.main.$fullpage.movePrev();
            },
            movePrev2() {
                this.$refs.main.$fullpage.moveTo(4);
            },
            movePrev3() {
                this.$refs.main.$fullpage.moveTo(2);
                this.$refs.main.$fullpage.movePrev();
            },
            movePrev4() {
                this.$refs.main.$fullpage.moveTo(1);
                this.$refs.main.$fullpage.movePrev();
            },
            moveNext() {
                this.$refs.main.$fullpage.moveNext();
            },
            moveNext2() {
                this.$refs.main.$fullpage.moveNext();
                this.$refs.main.$fullpage.moveNext();
            },
            moveNext3() {
                this.$refs.main.$fullpage.moveNext();
                this.$refs.main.$fullpage.moveNext();
                this.$refs.main.$fullpage.moveNext();
            },
            moveNext4() {
                this.$refs.main.$fullpage.moveNext();
                this.$refs.main.$fullpage.moveNext();
                this.$refs.main.$fullpage.moveNext();
                this.$refs.main.$fullpage.moveNext();
            }
        },
        components: {
            'v-member1': WTO,
            'v-member2': NI,
            'v-member3': pdd,
            'v-web': website,
            'v-web2': website2,
            'v-web3': website3,
            'v-wechat': wechat,
            'v-wechat2': wechat2,
            'v-wechat3': wechat3,
            'v-pro': pro,
            'v-pro2': pro2,
            'v-con': con
        }
    }
</script>

<style scoped>
    #app {
        height: 100vh;
        box-sizing: border-box;
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #fff;
    }
    .page-container {
        position: absolute;
        left: 0;
        right: 0;
        top: 0;
        width: 100%;
        height: 100%;
    }
    .guide {
        display: flex;
        width: 100%;
        height:15%;
    }
    .menuList1 {
        background: #2c3e50;
        margin: 5% 0 10px 20px;
        font-weight: bolder;
        border:none;
    }
    .menuList2 {
        background: #ffcc51;
        margin: 5% 0 10px 20px;
        font-weight: bolder;
        border:none;
    }
    .menuList3 {
        background: #030414;
        margin: 5% 0 10px 20px;
        font-weight: bolder;
        border:none;
    }
    .menuList4 {
        background: darkred;
        margin: 5% 0 10px 20px;
        font-weight: bolder;
        border:none;
    }
    .menuList5 {
        background: #0e863e;
        margin: 5% 0 10px 20px;
        font-weight: bolder;
        border:none;
    }

    .page-content {
        height: 100%;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .page-1{
        background-color:#2c3e50;
    }

    .page-2{
        background-color: #ffcc51;
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-around;
        align-items: center;
        flex-grow: 1;
    }
    .part-2{
        background-color: black;
        border-style: outset;
    }
    .page-3{
        background-color: #030414;

    }
    .page-4{
        background-color: darkred;
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-around;
        align-items: center;
        flex-grow: 1;
    }
     .page-4b {
         background-color: darkred;
         display: flex;
         flex-direction: row;
         flex-wrap: wrap;
         justify-content: space-around;
         align-items: center;
         flex-grow: 1;
     }
    .part-4{
        height:85%;
    }
    .part-32 {
        display:flex;
        justify-content: center;
        height: 50%;
        width: 100%;
    }
    .page-5{
        background-color: #0e863e;
    }


    .main-title {
        font-size: 6em;
        height:45%;
    }
    .title{
        width: 100%;
    }
</style>