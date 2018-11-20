<template>
    <b-card title="Cheney Ni" sub-title="鸡总" :img-src="url" img-alt="Image" img-top tag="article" style="max-width: 20rem;"
    class="mb-2">
        <p class="card-text">
            东方霍格沃滋密西根学院在读
        </p>
        <b-button href="https://github.com/nichujie">Github</b-button>
    </b-card>
</template>
<script>
export default {
    data () {
        return {
            url:require('../../assets/NI.jpg')
        }
    }
}
</script>
<style scoped>
</style>