<template>
    <h1>Non props</h1>
    <h2>{{ info }}</h2>
    <div v-bind="$attrs">
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Beatae velit minima alias eius error reprehenderit totam, obcaecati maxime provident quae, consequuntur architecto quo! Minima nisi pariatur excepturi itaque, sapiente autem. </p>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Beatae velit minima alias eius error reprehenderit totam, obcaecati maxime provident quae, consequuntur architecto quo! Minima nisi pariatur excepturi itaque, sapiente autem. </p>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Beatae velit minima alias eius error reprehenderit totam, obcaecati maxime provident quae, consequuntur architecto quo! Minima nisi pariatur excepturi itaque, sapiente autem. </p>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Beatae velit minima alias eius error reprehenderit totam, obcaecati maxime provident quae, consequuntur architecto quo! Minima nisi pariatur excepturi itaque, sapiente autem. </p>
        <h2>{{ info }}</h2>
    </div>
</template>

<script>
    export default{
        name: "non-props-component",
        props: {
            info: String,
        },
    }
</script>
