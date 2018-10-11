<template>
  <div id="app">
    <fullpage :options="options">
      <div class="section">
        
      </div>
      <div class="section">
      </div>
    </fullpage>
  </div>
</template>

<script>
import Fullpage from '';

export default {
  name: 'app',
  components: {
    FullPage
  },
  data () {
    return {
      options: {
        paddingTop: '30px'
      }
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
