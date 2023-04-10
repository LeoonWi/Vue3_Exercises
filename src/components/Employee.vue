<script>
    export default {
        emits: ['show1'],
        data() {
            return {
                
            };
        },
        methods: {
            Handel(name, salary) {
                this.$emit('show1', 'Данил', 'Ромашкан');
            },
        }
    }
</script>

<template>
   <button @click="Handel">Имя и оклад</button>
</template>