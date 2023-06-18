<template>
    <h1>Student: {{ name }}</h1>
</template>

<script>
   export default {
       name: "student-component",
       props: {
            name: String,
       },
   };
</script>