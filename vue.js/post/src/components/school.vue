<template>
    <h1>School</h1>
    <h1>{{ childUser }}</h1>
    <TeacherComponent name="Bruce" :getUser="getUserName"/>
    <StudentComponent name="Leo"/>
</template>

<script>
    import StudentComponent from './student.vue'
    import TeacherComponent from './teacher.vue'

    export default {
        name: "school-component",
        components: {
            StudentComponent,
            TeacherComponent,
        },
        methods: {
            getUserName(name) {
                this.childUser = name;
            },
        },
        data() {
            return {
                childUser: "",
            }
        }
    };
</script>
