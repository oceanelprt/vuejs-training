<template>
    <h1>Watcher</h1>
    <h2>Counter</h2>
    {{ counter }}
    <br />
    <button v-on:click="counter = counter + 1">+</button>
    <button v-on:click="counter = counter - 1">-</button>

    <!-- <ChildSlotComponent>
    <h1>Hello there !</h1>
    </ChildSlotComponent>
    <ChildSlotComponent>
        <h1>General Kenobi</h1>
    </ChildSlotComponent>
    <ChildSlotComponent>
        <img src="https://media.tenor.com/smu7cmwm4rYAAAAC/general-kenobi-kenobi.gif" alt="GIF Hello There General Kenobi"/>
    </ChildSlotComponent>
    <ChildSlotComponent></ChildSlotComponent> -->

    <ChildSlotComponent>
        <template v-slot:header><h1>First Heading</h1></template>
        <template v-slot:section><h3>Product</h3></template>
        <template v-slot:main><h3>Name</h3></template>
        <template v-slot:footer><h2>Price</h2></template>
    </ChildSlotComponent>

    <ChildSlotComponent>
        <template v-slot:header><h1>Brand</h1></template>
        <template v-slot:section><h3>Product</h3></template>
        <template v-slot:main><h3>Name</h3></template>
        <template v-slot:footer><h2>Price</h2></template>
    </ChildSlotComponent>
</template>

<script>
    import ChildSlotComponent from './child-slot.vue'

    export default {
        name: "watcher-component",
        data() {
            return {
                counter: 0,
            }
        },
        components: {
            ChildSlotComponent,
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
