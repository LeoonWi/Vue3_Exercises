<script>
    export default {
        props: {
            id: Number,
            name: String,
            salary: Number,
            age: Number
        },
        data() {
            return {
                
            }
        },
    }
</script>

<template>
   <p>{{ id }} {{ name }} {{ salary }} {{ age }}</p><br>
</template>