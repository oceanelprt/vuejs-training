<template>
    <h1>Hello there {{ "hello".length }}</h1>
    <h1>Email {{ email }}</h1>
    <h1>Name {{ getName1() }}</h1>
    <h1>Name {{ getName2("Helio") }}</h1>
    <h1>Name {{ getName("Carlosse") }}</h1>
    <h1>Name {{ getName("Joe") }}</h1>
    <h1>Data : {{ getData() }}</h1>
    <h1>Data email : {{ getData().email }}</h1>
    <h1>Data phone : {{ getData().mobile }}</h1>
    <button v-on:click="fun()">Click for fun !</button>
    <button v-on:dblclick="getData2('hello')">Click here !</button>
    <h1 v-on:mousemove="getConsole()">Homepage</h1>
</template>

<script>
    export default{
        name: "PAGES",
        data() {
            return {
                email: "abcd@gmail.com",
                mobile: "55555",
                getName1: function(){
                    return "Oceane";
                },
                getName2: function(name){
                    return name;
                }
            }
        },
        methods:{
            getName(name){
                return name;
            },
            getData(){
                return {
                    email: this.email,
                    mobile: this.mobile,
                }
            },
            fun(){
                alert("How are you ?");
            },
            getData2(data){
                alert(data);
            },
            getConsole() {
                console.log("Function is running");
            }
        },
    }
</script>

<style scoped>
h1 {
    color: red;
}
</style>