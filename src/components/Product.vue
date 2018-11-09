<template>
    <div>
    <b-card-group columns>
        <b-card img-src="https://placekitten.com/g/400/450"
                img-fluid
                img-alt="image"
                img-top>
            <p class="text-muted">context context context context context context context context</p>
        </b-card>
        <b-card
                :img-src="url"
                img-fluid
                text-variant="dark"
                img-alt="image"
                img-top>
            <p class="text-muted">context context context context context context context context</p>
            <div>
                  <b-btn v-b-toggle.collapse1 variant="primary">click here</b-btn>
                  <b-collapse id="collapse1" class="mt-2">
                    <b-card>
                      <p class="card-text">For more details</p>
                      <b-btn href="www.baodu.com" v-b-toggle.collapse1_inner size="sm">github</b-btn>
                    </b-card>
                  </b-collapse>
            </div>
        </b-card>
        <b-card bg-variant="primary"
                text-variant="white">
            <blockquote class="card-blockquote">
                <footer>
                    <small>context context context context<cite title="Source Title"></cite></small>
                </footer>
            </blockquote>
        </b-card>
        <b-card title="Title">
            <p class="text-muted">context context context context context context context context</p>
        </b-card>
        <b-card overlay
                img-src="https://picsum.photos/400/400/?image=41"
                img-fluid
                img-alt="image"
                >
            <p>
                context context
            </p>
        </b-card>

    </b-card-group>
</div>

</template>

<script>
    export default {
        data(){
            return {
                url:require("../assets/contact.jpg")
            }
        }
    }
</script>

<style scoped>

</style>