<script>
    export default {
        props: {
            name: String,
            surname: String,
            age: Number
        },
        data() {
            return {
                
            }
        },
    }
</script>

<template>
    <p>{{ name }}</p><br>
    <p>{{ surname }}</p><br>
    <p>{{ age }}</p>
</template>