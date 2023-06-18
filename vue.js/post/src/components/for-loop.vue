<template>
    <h1 id="page-for-loop">For loop</h1>
    <ul>
        <li v-for="program in technology" :key="program">
            {{ program }}
        </li>
    </ul>
    <br/>
    <ul>
        <li v-for="data in user" :key="data">
            Name is : {{ data.name }}
        </li>
        <li v-for="data in user" :key="data">
            Email is : {{ data.email }}
        </li>
        <li v-for="data in user" :key="data">
            Contact is : {{ data.contact }}
        </li>
    </ul>

    <Child name="Tony Stark" :userTony="userTony" :getData="getData"/>
</template>

<script>
    import Child from './child.vue'
    export default {
        name: "for-loop",
        data() {
            return {
                technology: ["PHP", "Javascript", "C++", "C-sharp"],
                user: [
                    {
                        name: "Jack",
                        email: "jack@gmail.com",
                        contact: +948548855484
                    },
                    {
                        name: "Son",
                        email: "son@gmail.com",
                        contact: +84520252
                    },
                    {
                        name: "Mickael",
                        email: "mickael@gmail.com",
                        contact: +5651548548
                    },
                ],
                userTony:
                {
                    name: "Tony",
                    email: "tony@gmail.com",
                    contact: +5651548548
                },
            };
        },
        components: {
            Child,
        },
        methods: {
            getData(){
                alert("Method called");
            },
        }
    };
</script>

<style scoped>
    h1 {
        color:maroon;
    }
</style>
