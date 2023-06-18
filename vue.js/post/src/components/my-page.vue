<template>
    <h1>Two way Binding</h1>
    <input type="text" placeholder="Add the number" v-model="count">
    <h3>{{ count }}</h3>
</template>

<script>
    export default {
        name: "My-page",
        data() {
            return {
                count: 7,
            }
        }
    };
</script>

<style scoped>
    h1 {
        color:blue;
    }
</style>
