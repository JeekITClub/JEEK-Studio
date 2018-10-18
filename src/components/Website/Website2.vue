<template>
    <div class="wechat">
        <div>
          <b-card overlay
                  :img-src="url"
                  img-alt="Card Image"
                  text-variant="white"
                  title="开发网页">
            <p class="card-text">
              认真负责的成员将会按照你们的要求编写网站
                <br>
             第二行
                <br>
                第三行
            </p>
          </b-card>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return{
                url:require("../../assets/website.jpg")
            }
        }
    }
</script>

<style scoped>

</style>