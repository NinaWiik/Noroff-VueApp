<template>
  <div id="app">
    <h1>Recepies</h1>
    <recipePage />
    <router-view></router-view>
  </div>
</template>

<script>
import recipePage from './components/recipePage.vue'

export default {
  name: 'App',
  components: {
    recipePage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: black;
  margin: 0;
}

</style>
