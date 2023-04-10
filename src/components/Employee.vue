<script>
    export default {
        props: ['arr'],
        data() {
            return {
                
            }
        },
    }
</script>

<template>
    <ul>
        <li v-for="elem in arr">{{ elem }}</li>
    </ul>
</template>