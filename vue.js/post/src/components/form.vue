<template>
    <h1>Simple form</h1>
    <form action="">
        <label for="">Username</label>&nbsp;
        <input type="text" name="" id="" placeholder="username" v-model="form.username">
        <br/>
        <br/>
        <label for="">Password</label>&nbsp;&nbsp;
        <input type="password" name="" id="" v-model="form.password">
        <br/>
        <br/>
        <label for="">Hobbies</label>&nbsp;&nbsp;
        <label for="basketball">Basketball</label>&nbsp;&nbsp;
        <input type="checkbox" name="" id="basketball" value="basketball" v-model="form.hobbies">
        <label for="horse-riding">Horse riding</label>&nbsp;&nbsp;
        <input type="checkbox" name="" id="horse-riding" value="horse-riding" v-model="form.hobbies">
        <label for="golf">Golf</label>&nbsp;&nbsp;
        <input type="checkbox" name="" id="golf" value="golf" v-model="form.hobbies">
        <br/>

        <label for="">Gender</label>&nbsp;&nbsp;
        <label for="">Male</label>&nbsp;&nbsp;
        <input type="radio" name="gender" id="" value="male" v-model="form.gender">
        <label for="">Female</label>&nbsp;&nbsp;
        <input type="radio" name="gender" id="" value="female" v-model="form.gender">
        <br/>
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
                    hobbies: [],
                    gender: "",
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
