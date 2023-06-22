<template>
    <h1 ref="removing">Before unmount & unmounted</h1>
    <button @click="active = 'WatcherComponent'">Watcher</button>
    <button @click="active = 'SchoolComponent'">School</button>
    <button @click="active = 'IfElseCondition'">If else</button>
    <button @click="active = 'ForLoop'">For loop</button>

    <!-- <WatcherComponent/>
    <SchoolComponent/>
    <IfElseCondition/>
    <ForLoop/> -->

    <component :is="active"/>
    <Teleport to="#header">
        <HeaderComponent/>
    </Teleport>
</template>

<script>
    import WatcherComponent from './watcher.vue';
    import SchoolComponent from './school.vue';
    import IfElseCondition from './if-else.vue';
    import ForLoop from './for-loop.vue';
    import HeaderComponent from './header.vue';

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
            HeaderComponent,
        },
        beforeUnmount() {
            console.log('beforeUnmount', this.$refs['removing']);
        },
        unmounted() {
            console.log('unmounted', this.$refs['removing']);
        },
    };
</script>
