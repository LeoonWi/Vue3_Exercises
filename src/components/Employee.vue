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
    <p>{{ surname }}</p><br>
    <p>{{ name }}</p><br>
    <p>{{ age }}</p>
</template>