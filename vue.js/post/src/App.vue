<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h1 ref="counter">Count : {{ count }}</h1>
  <button v-on:click="count = count + 1">Up</button>

  <br /><br />
<!--   <NewOne />
  <MyPage />
  <InputBoxes />
  <IfElseCondition />
  <ForLoop />
  <SchoolComponent />
  <FormComponent />
  <PropsComponent />
  <ComputedPropertyComponent />
  <WatcherComponent />-->
  <HomeComponent/>
</template>

<script>
/*   import NewOne from './components/New-onef.vue'
  import MyPage from './components/my-page.vue'
  import InputBoxes from './components/input-boxes.vue'
  import IfElseCondition from './components/if-else.vue'
  import ForLoop from './components/for-loop.vue'
  import SchoolComponent from './components/school.vue'
  import FormComponent from './components/form.vue'
  import PropsComponent from './components/props.vue'
  import ComputedPropertyComponent from './components/computed-property.vue'
  import WatcherComponent from './components/watcher.vue'
*/
  import HomeComponent from './components/home.vue'

  export default {
    name: 'App',
    components: {
/*       NewOne,
      MyPage,
      InputBoxes,
      IfElseCondition,
      ForLoop,
       SchoolComponent,
       FormComponent,
       PropsComponent,
       ComputedPropertyComponent, 
       WatcherComponent,*/
       HomeComponent,
    },
    data() {
      console.log('created');
      return {
        count: 0,
      };
    },
    // beforeCreate() {
    //   alert('Loading...');
    // },
    // created() {
    //   alert('Loaded');
    // },
    // beforeMount() {
    //   console.log("This is a beforeMount methode", this.$el);
    // },
    // mounted() {
    //   console.log("This is a mounted methode", this.$el);
    // },
    beforeUpdate() {
      console.log("beforeUpdate", this.$refs['counter'].textContent);
    },
    updated() {
      console.log("Updated", this.count);
    },
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
