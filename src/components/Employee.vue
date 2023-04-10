<script>
    export default {
        props: {
            id: Number,
            name: String,
            surn: String
        },
        emits: ['remove'],
        data() {
            return {
                
            };
        },
    }
</script>

<template>
   <p>{{ name }} {{ surn }}</p><br>
   <button @click="$emit('remove', id)">Удалить</button><br>
</template>