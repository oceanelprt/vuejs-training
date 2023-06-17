<template>
    <h1>How to add Two way Binding in multiple input boxes</h1>

    <label for="cricket">Cricket</label>
    &nbsp;
    <input type="checkbox" value="cricket" id="" v-model="sports" />
    <br />

    <label for="football">Football</label>
    &nbsp;
    <input type="checkbox" value="football" id="" v-model="sports" />
    <br />

    <label for="basketball">Basketball</label>
    &nbsp;
    <input type="checkbox" value="basketball" id="" v-model="sports" />
    <br />

    <label for="">Player name</label>
    &nbsp; &nbsp;
    <label for="name1">Obasohan</label>
    &nbsp;
    <input type="radio" value="Obasohan" id="name1" name="player" v-model="player">

    <label for="name2">Grizemann</label>
    &nbsp;
    <input type="radio" value="Griezmann" id="name2" name="player" v-model="player">

    <h3>Selected sports : {{ sports }}</h3>
    <h3>Selected player : {{ player }}</h3>

</template>

<script>
    export default {
        name: "Input-boxes",
        data() {
            return {
                sports: [],
                player: [],
            }
        }
    };
</script>

<style scoped>
    h1 {
        color:green;
    }
</style>
