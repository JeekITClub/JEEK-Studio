<template>
    <div class="wechat">
        <div>
          <b-card overlay
                  :img-src="url"
                  img-alt="Card Image"
                  text-variant="white"
                  title="沟通与调试">
            <p class="card-text">
              当项目每个阶段初步完成之后我们会与<br>
                客户进行沟通并且按照客户的要求
                <br>
              进行修改。
            </p>
          </b-card>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return{
                url:require("../../assets/communication.png")
            }
        }
    }
</script>

<style scoped>

</style>