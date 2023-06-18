<template>
     <div class="user-component">
        <h2>{{ user.name }}</h2>
        <h2>{{ user.email }}</h2>
    </div>
 </template>

<script>
    export default {
        name: "new-user",
        props: {
            user: Object,
        },
    };
</script>

<style scoped>
    h2 {
        color:lightcoral;
    }
    .user-component {
        padding:12px;
        margin-bottom: 15px;
        border: 1px solid;
        background-color: blanchedalmond;
    }
</style>
