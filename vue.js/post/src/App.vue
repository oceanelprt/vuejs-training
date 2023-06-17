<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <PAGES />
</template>

<script>
import PAGES from './components/New-onef.vue'

export default {
  name: 'App',
  components: {
    PAGES,
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
  margin-top: 60px;
}
</style>
