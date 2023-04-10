<script>
    export default {
        props: ['name', 'surname', 'age'],
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