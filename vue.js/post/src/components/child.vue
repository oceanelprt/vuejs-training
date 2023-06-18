<template>
    <h1 id="page-child">Child component</h1>
    <h3>{{ name }}</h3>
    <h3>{{ userTony.email }}</h3>
    <button v-on:click="getData()">Call the function</button>
</template>

<script>
    export default {
        name: "child-component",
        props: {
            name: String,
            userTony: Object,
            getData: Function,
        }
    };
</script>

<style scoped>
    h3 {
        color:blue;
        font-weight: bold;
    }
</style>
