<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
  (function () {
    localStorage.setItem('username', 'Nina');
    localStorage.setItem('password', '1234');
  })();
  
export default {
  name: 'App',
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: lightgrey;
  margin: 0;
}

</style>
