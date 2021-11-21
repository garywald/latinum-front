<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/latinum_logo.png">
    <Latinum msg="List of the humans welcomed to the Latinum"/>
  </div>
</template>

<script>
import Latinum from './components/Latinum.vue'

export default {
  name: 'app',
  components: {
    Latinum
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
