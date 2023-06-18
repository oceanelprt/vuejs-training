<template>
    <h1 id="page-child">Child component</h1>
    <h3>{{ name }}</h3>
    <h3>{{ userTony.email }}</h3>
    <button v-on:click="getData()">Call the function</button>

    <ul>
        <li v-for="user in users" :key="user.name">
            <newUser :user="user"/>
        </li>
    </ul>
    <h1 v-html="peterEmail"></h1>
    <div v-html="peterId"></div>
    <newUser />
</template>

<script>
    import newUser from './new-user.vue';

    export default {
        name: "child-component",
        props: {
            name: String,
            userTony: Object,
            getData: Function,
        },
        data() {
            return {
                users: [
                    {
                        name:'Jackson',
                        email: 'jackson5@gmail.com',
                    },
                    {
                        name:'Smith',
                        email: 'smith@gmail.com',
                    },
                    {
                        name:'John',
                        email: 'john@gmail.com',
                    },
                    {
                        name:'athan',
                        email: 'athan@gmail.com',
                    },
                    {
                        name:'Oliver',
                        email: 'oli@gmail.com',
                    },
                ],
                peterName: 'Peter',
                peterEmail: '<h3>peter123@gmail.com</h3>',
                peterId: '<h1>26556</h1>',
            };
        },
        components: {
            newUser,
        },
    };
</script>

<style>
    h3 {
        color:blue;
        font-weight: bold;
    }
</style>
