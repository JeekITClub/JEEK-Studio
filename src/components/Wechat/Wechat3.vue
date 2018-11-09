<template>
    <div class="wechat">
        <div>
          <b-card overlay
                  :img-src="url"
                  img-alt="Card Image"
                  text-variant="dark"
                  title="项目需求">
            <p class="card-text">
              context context context context
                <br>context contextcontext context
                <br>context contextcontext context
            </p>
          </b-card>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return{
                url:require("../../assets/backboard.png")
            }
        }
    }
</script>

<style scoped>

</style>