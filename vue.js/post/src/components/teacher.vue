<template>
    <h1>Teacher: {{ name }}</h1>
    <button v-on:click="getUser(userName)">Get the name</button>
</template>

<script>
   export default {
       name: "teacher-component",
       props: {
            name: String,
            getUser: Function,
       },
       data() {
        return {
            userName: "Clark",
        }
       }
   };
</script>
