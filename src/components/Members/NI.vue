<template>
    <div class="member">
     <div>
        <b-card title="WTO"
                sub-title="台长"
          :img-src="url"
          img-alt="Image"
          img-top
          bg-variant="dark"
          tag="article"
          style="max-width: 20rem;"
          class="mb-2">
        <p class="card-text" >
        Please write down self-introduction here and something like that balabalabalabalabalabal.bababalla lansdn lasjdkn alsda nsdaknsdkan s
        </p>
        <b-button href="https://github.com/alienmao" >Github</b-button>
        </b-card>
     </div>
    </div>
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
    .mb-2{

    }
</style>