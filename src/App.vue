<script>
  export default {
    data() {
      return {
        items: [1, -2, 3, -4, 5],
      }
    },
    methods: {
      
    }    
  }
</script>

<template>
  <template v-for="elem in items">
    <p v-if="elem >= 0">{{ elem }}</p>
  </template>
 </template>

<style>

</style>