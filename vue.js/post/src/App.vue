<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <NewOne />
  <MyPage />
  <InputBoxes />
</template>

<script>
import NewOne from './components/New-onef.vue'
import MyPage from './components/my-page.vue'
import InputBoxes from './components/input-boxes.vue'

export default {
  name: 'App',
  components: {
    NewOne,
    MyPage,
    InputBoxes
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
