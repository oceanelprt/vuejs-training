<template>
    <button @click="active = 'WatcherComponent'">Watcher</button>
    <button @click="active = 'SchoolComponent'">School</button>
    <button @click="active = 'IfElseCondition'">If else</button>
    <button @click="active = 'ForLoop'">For loop</button>

    <!-- <WatcherComponent/>
    <SchoolComponent/>
    <IfElseCondition/>
    <ForLoop/> -->

    <component :is="active"/>
</template>

<script>
    import WatcherComponent from './watcher.vue';
    import SchoolComponent from './school.vue';
    import IfElseCondition from './if-else.vue';
    import ForLoop from './for-loop.vue';

    export default {
        name: "home-component",
        data() {
            return {
                active: 'WatcherComponent',
            }
        },
        components: {
            WatcherComponent,
            SchoolComponent,
            IfElseCondition,
            ForLoop,
        },
    };
</script>
