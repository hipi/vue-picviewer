<template>
  <div id="app">
    <Picview/>
  </div>
</template>

<script>
import Picview from './Picview.vue'

export default {
  name: 'app',
  components: {
    Picview
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
body{
  margin: 0;
  padding: 0;
}
</style>
