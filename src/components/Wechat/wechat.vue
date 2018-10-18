<template>
    <div class="wechat">
        <div>
          <b-card overlay
                  :img-src="url"
                  img-alt="Card Image"
                  text-variant="white"
                  title="项目需求">
            <p class="card-text">
              在项目编写开始之前我们会详细的
                <br>记录客户对于网站功能要求以及偏
                <br>爱的网站风格
            </p>
          </b-card>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return{
                url:require("../../assets/contact.jpg")
            }
        }
    }
</script>

<style scoped>

</style>