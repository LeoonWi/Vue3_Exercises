<script>
    export default {
        emits: ['show1', 'show2'],
        data() {
            return {
                
            };
        },
        methods: {
            HandelName() {
                this.$emit('show1');
            },
            HandelSalary() {
                this.$emit('show2');
            },
        }
    }
</script>

<template>
   <button @click="HandelName">Name</button>
   <button @click="HandelSalary">Salary</button>
</template>