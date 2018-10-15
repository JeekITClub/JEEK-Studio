<template>
    <div id="app">
        <div class="page-container">
            <div class="fullpage-wp" v-fullpage="opts" ref="main">
                <div class="page-1 page">
                    <b-button-group class="guide">
                            <b-button  class="menuList1">首页</b-button>
                            <b-button @click="moveNext" class="menuList1" >主要业务介绍</b-button>
                            <b-button @click="moveNext2" class="menuList1">主要作品</b-button>
                            <b-button @click="moveNext3" class="menuList1">人员介绍</b-button>
                            <b-button @click="moveNext4" class="menuList1">主要联系方式</b-button>
                    </b-button-group>
                    <div class="page-content">
                        <h1 class="part-1 main-title" v-animate="{value: 'bounceInLeft'}">Jeek Studio</h1>
                    </div>
                </div>
                <div class="page-2 page">
                        <b-button-group class="guide">
                            <b-button @click="movePrev" class="menuList2">首页</b-button>
                            <b-button class="menuList2" >主要业务介绍</b-button>
                            <b-button @click="moveNext" class="menuList2">主要作品</b-button>
                            <b-button @click="moveNext2" class="menuList2">人员介绍</b-button>
                            <b-button @click="moveNext3" class="menuList2">主要联系方式</b-button>
                        </b-button-group>
                        <v-member1  class="part-2" v-animate="{value: 'bounceInLeft', delay: 1200}"></v-member1>
                        <v-member2  class="part-2" v-animate="{value: 'zoomInDown', delay: 0}"></v-member2>
                        <v-member3  class="part-2" v-animate="{value: 'bounceInRight', delay: 600}"></v-member3>

                </div>
                <div class="page-3 page">
                    <b-button-group class="guide">
                            <b-button @click="movePrev2" class="menuList3">首页</b-button>
                            <b-button @click="movePrev" class="menuList3" >主要业务介绍</b-button>
                            <b-button  class="menuList3">主要作品</b-button>
                            <b-button @click="moveNext" class="menuList3">人员介绍</b-button>
                            <b-button @click="moveNext2" class="menuList3">主要联系方式</b-button>
                    </b-button-group>
                    <p class="part-3" v-animate="{value: 'bounceInLeft', delay: 0}">fullpage-vue</p>
                    <p class="part-3" v-animate="{value: 'bounceInRight', delay: 600}">fullpage-vue</p>
                    <p class="part-3" v-animate="{value: 'zoomInDown', delay: 1200}">fullpage-vue</p>
                </div>
                 <div class="page-4 page">
                     <b-button-group class="guide">
                            <b-button @click="movePrev3" class="menuList4">首页</b-button>
                            <b-button @click="movePrev2" class="menuList4" >主要业务介绍</b-button>
                            <b-button @click="movePrev" class="menuList4">主要作品</b-button>
                            <b-button  class="menuList4">人员介绍</b-button>
                            <b-button @click="moveNext" class="menuList4">主要联系方式</b-button>
                     </b-button-group>
                    <p class="part-4" v-animate="{value: 'bounceInLeft', delay: 0}">fullpage-vue</p>
                    <p class="part-4" v-animate="{value: 'bounceInRight', delay: 600}">fullpage-vue</p>
                    <p class="part-4" v-animate="{value: 'zoomInDown', delay: 1200}">fullpage-vue</p>
                </div>
                 <div class="page-5 page">
                     <b-button-group class="guide">
                            <b-button @click="movePrev4" class="menuList5">首页</b-button>
                            <b-button @click="movePrev3" class="menuList5" >主要业务介绍</b-button>
                            <b-button @click="movePrev2" class="menuList5">主要作品</b-button>
                            <b-button @click="movePrev" class="menuList5">人员介绍</b-button>
                            <b-button class="menuList5">主要联系方式</b-button>
                     </b-button-group>
                    <p class="part-5" v-animate="{value: 'bounceInLeft', delay: 0}">fullpage-vue</p>
                    <p class="part-5" v-animate="{value: 'bounceInRight', delay: 600}">fullpage-vue</p>
                    <p class="part-5" v-animate="{value: 'zoomInDown', delay: 1200}">fullpage-vue</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import WTO from "./WTO"
    import NI from "./NI"
    import pdd from "./PDD"
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
        methods: {
            movePrev() {
                this.$refs.main.$fullpage.movePrev();
            },
            movePrev2() {
                this.$refs.main.$fullpage.movePrev();
                this.$refs.main.$fullpage.movePrev();
            },
            movePrev3() {
                this.$refs.main.$fullpage.movePrev();
                this.$refs.main.$fullpage.movePrev();
                this.$refs.main.$fullpage.movePrev();
            },
            movePrev4() {
                this.$refs.main.$fullpage.movePrev();
                this.$refs.main.$fullpage.movePrev();
                this.$refs.main.$fullpage.movePrev();
                this.$refs.main.$fullpage.movePrev();
            },
            moveNext() {
                this.$refs.main.$fullpage.moveNext(); //Move to the next page
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
            'v-member3': pdd
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
        length: 20px;
    }
    .menuList1 {
        background: #2c3e50;
        margin: 60px 0 0 20px;
        font-weight: bolder;
    }
    .menuList2 {
        background: #ffcc51;
        margin: 0 0 0 20px;
        font-weight: bolder;
    }
    .menuList3 {
        background: blueviolet;
        margin: 60px 0 0 20px;
        font-weight: bolder;
    }
    .menuList4 {
        background: darkred;
        margin: 60px 0 0 20px;
        font-weight: bolder;
    }
    .menuList5 {
        background: aqua;
        margin: 60px 0 0 20px;
        font-weight: bolder;
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
        background-color:blueviolet;
    }
    .page-4{
        background-color: darkred;
    }
    .page-5{
        background-color: aqua;
    }


    .main-title {
        font-size: 6em;
    }
</style>