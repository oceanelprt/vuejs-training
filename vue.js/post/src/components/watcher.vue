<template>
    <h1>Watcher</h1>
    <h2>Counter</h2>
    {{ counter }}
    <br />
    <button v-on:click="counter = counter + 1">+</button>
    <button v-on:click="counter = counter - 1">-</button>
</template>

<script>
    export default {
        name: "watcher-component",
        data() {
            return {
                counter: 0,
            }
        },
        watch: {
            counter(num, last) {
                if (num > 10 && num > last) {
                    alert ("10 is maximum number");
                    this.counter = 0;
                }
            },
        },
    };
</script>
