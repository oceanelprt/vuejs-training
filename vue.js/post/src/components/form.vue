<template>
    <h1>Simple form</h1>
    <form action="">
        <label for="">Username</label>&nbsp;
        <input type="text" name="" id="" placeholder="username" v-model="form.username">
        <br/>
        <label for="">Password</label>&nbsp;
        <input type="password" name="" id="" v-model="form.password">
        <br/>
        <button v-on:click="login()">Sign up</button>

        <p>{{ form }}</p>
    </form>
</template>

<script>
    export default{
        name: "form-component",
        data() {
            return {
                form : {
                    username:"",
                    password:"",
                }
            }
        },
        methods:{
            login(){
                console.log(this.form)
            }
        },
    }
</script>
