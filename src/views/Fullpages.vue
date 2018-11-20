<template>
    <page3></page3>
    <!-- <div class="fullpage-container">
        <div class="fullpage-wp" v-fullpage="opts" ref="example">
            <div class="page-1 page">
                <p class="part-1" v-animate="{value: 'bounceInLeft'}">
                    fullpage-vue1
                </p>
            </div>
            <div class="page-2 page">
                <p class="part-2" v-animate="{value: 'bounceInRight'}">
                    fullpage-vue2
                </p>
            </div>
            <div class="page-3 page">
                <p class="part-3" v-animate="{value: 'bounceInLeft', delay: 0}">
                    <page3></page3>
                </p>
            </div>
        </div>
        <button @click="moveNext">next</button>
    </div> -->
</template>

<script>
    import page3 from './pages/page3'
    export default {
        components: {
            page3
        },
        data() {
            return {
                opts: {
                    start: 0,
                    dir: 'v',
                    duration: 500
                    // beforeChange: function (prev, next) {},
                    // afterChange: function (prev, next) {}
                }
            }
        },
        method: {
            moveNext() {
                this.$refs.example.$fullpage.moveNext(); //Move to the next page
            }
        }
    }
</script>

<style>

</style>