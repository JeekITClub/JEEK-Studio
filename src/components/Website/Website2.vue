<template>
    <div class="wechat">
        <div>
          <b-card overlay
                  :img-src="url"
                  img-alt="Card Image"
                  text-variant="dark"
                  title="开发网页">
            <p class="card-text">
              context contextcontext contextcontext context
                <br>
             context contextcontext context
                <br>
                context contextcontext context
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