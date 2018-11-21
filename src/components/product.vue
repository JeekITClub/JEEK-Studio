<template>
    <div class="product-card">
        <div class="img">
            <img :src="url">
        </div>
        <div class="title">
            {{ title }}
        </div>
        <div class="desc">
            {{ desc }}
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return {}
    },
    props: {
        url: String,
        desc: String,
        title: String
    }
}
</script>


<style lang="scss" scoped>
    .product-card {
        width: 100%;
        .title {
            font-size: 1.5rem;
            margin-top: 1vh;
            margin-bottom: 1vh;
            text-align: center;
        }
        .desc {
            font-size: 1rem;
            text-align: center;
        }
        .img {
            text-align: center;
            width: 100%;
        }
    }
</style>
