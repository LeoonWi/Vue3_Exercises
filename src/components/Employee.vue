<script>
    export default {
        emits: ['show1'],
        data() {
            return {
                
            };
        },
    }
</script>

<template>
   <button @click="$emit('show1', 'Данил', 'Ромашкан')">Имя и оклад</button>
</template>