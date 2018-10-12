<template>
    <div id="app">
        <div class="page-container">
            <div class="fullpage-wp" v-fullpage="opts" ref="main">
                <div class="page-1 page">
                    <div class="page-content">
                        <h1 class="part-1 main-title" v-animate="{value: 'bounceInLeft'}">Jeek Studio</h1>
                    </div>
                </div>
                <div class="page-2 page">
                    <p class="part-2" v-animate="{value: 'bounceInLeft', delay: 0}">fullpage-vue</p>
                    <p class="part-2" v-animate="{value: 'bounceInRight', delay: 600}">fullpage-vue</p>
                    <p class="part-2" v-animate="{value: 'zoomInDown', delay: 1200}">fullpage-vue</p>
                </div>
                <div class="page-3 page">
                    <p class="part-3" v-animate="{value: 'bounceInLeft', delay: 0}">fullpage-vue</p>
                    <p class="part-3" v-animate="{value: 'bounceInRight', delay: 600}">fullpage-vue</p>
                    <p class="part-3" v-animate="{value: 'zoomInDown', delay: 1200}">fullpage-vue</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

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
            moveNext() {
                this.$refs.main.$fullpage.moveNext(); //Move to the next page
            }
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
        top: 0;
        width: 100%;
        height: 100%;
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
        background-color: coral;
    }

    .page-3{
        background-color:blueviolet;
    }

    .main-title {
        font-size: 6em;
    }
</style>