<template>
    <h1 id="page-if-condition" v-if="display">If condition</h1>
    <h1 id="page-if-condition" v-else>Else condition 2</h1>
    <button v-on:click="display = !display">Click here</button>
</template>

<script>
    export default {
        name: "if-else-condition",
        data() {
            return {
                display: true,
                show: true,
            };
        }
    };
</script>

<style scoped>
    h1 {
        color:pink;
    }
</style>
