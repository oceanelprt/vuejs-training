<template>
    <h1>Slots</h1>
    <div id="product-card">
        <header><slot name="header"></slot></header>
        <section><slot name="section"></slot></section>
        <main><slot name="main"></slot></main>
        <footer><slot name="footer"></slot></footer>
    </div>
</template>

<script>
    export default {
        name: "slot-child-component",
    };
</script>

<style>
    #product-card {
        width: 400px;
        padding: 2px;
        text-align: center;
        border: 1px solid;
        background-color: beige;
    }
</style>
