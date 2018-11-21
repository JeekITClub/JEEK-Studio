<template>
    <div class="member-card">
        <img :src="url" class="img mx-auto d-block">
        <div class="name">
            {{ name }}
        </div>
        <div class="desc">
            {{ desc }}
        </div>
    </div>
</template>

<script>
export default {
    props: {
        url: String,
        name: String,
        desc: String
    }
}
</script>

<style lang="scss" scoped>
    .member-card {
        padding: 2vh;
        margin: 5vh;
        .img {
            margin-top: -6vh;
            height: 100%;
            box-shadow: -4px 6px 12px 1px #888888;
            border-radius: 100%;
        }
        .name {
            margin-top: 1vh;
            text-align: center;
            font-size: 2rem;
        }
        .desc {
            text-align: center;
            font-size: 1rem;
        }
    }  
</style>
