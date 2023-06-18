<template>
    <h1>Props</h1>
    <NonPropsComponent info="Hello World" id="name" />
</template>

<script>
    import NonPropsComponent from './non-props.vue'

    export default{
        name: "props-component",
        components:{
            NonPropsComponent,
        }
    }
</script>
