<template>
    <div class="plan-card">
        {{ price }}
    </div>
</template>

<script>
export default {
    props: {
        price: Number
    }
}
</script>

<style lang="scss" scoped>
    .plan-card {
        &:hover {
            color: white;
            background: black;
        }
        color: black;
    }
</style>
