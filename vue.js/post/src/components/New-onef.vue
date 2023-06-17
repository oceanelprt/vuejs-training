<template>
    <h1>Hello there {{ "hello".length }}</h1>
    <h1>Email {{ email }}</h1>
    <h1>Number {{ mobile = 111 }}</h1>
    <h1>Name {{ getName1() }}</h1>
    <h1>Name {{ getName2("Helio") }}</h1>
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
        }
    }
</script>

<style scoped>
h1 {
    color: red;
}
</style>