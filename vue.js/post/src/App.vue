<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <NewOne />
  <MyPage />
  <InputBoxes />
  <IfElseCondition />
  <ForLoop />
</template>

<script>
  import NewOne from './components/New-onef.vue'
  import MyPage from './components/my-page.vue'
  import InputBoxes from './components/input-boxes.vue'
  import IfElseCondition from './components/if-else.vue'
  import ForLoop from './components/for-loop.vue'

  export default {
    name: 'App',
    components: {
      NewOne,
      MyPage,
      InputBoxes,
      IfElseCondition,
      ForLoop,
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
