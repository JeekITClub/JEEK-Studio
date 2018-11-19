<template>
    <div class="fullpage-container">
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
                    fullpage-vue3
                </p>
                <p class="part-3" v-animate="{value: 'bounceInRight', delay: 600}">
                    fullpage-vue4
                </p>
                <p class="part-3" v-animate="{value: 'zoomInDown', delay: 1200}">
                    fullpage-vue5
                </p>
            </div>
        </div>
        <button @click="moveNext">next</button>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                opts: {
                    start: 0,
                    dir: 'v',
                    duration: 500,
                    beforeChange: function (prev, next) {},
                    afterChange: function (prev, next) {}
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