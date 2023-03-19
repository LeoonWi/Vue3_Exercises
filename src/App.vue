<script>
  export default {
    data() {
      return {
        arr: ['x', 'y', 'z'],
      }
    },
    methods: {
      
    }    
  }
</script>

<template>
  <div>
    <ul><li v-for="(n, k) in arr">{{ n }}</li></ul>
  </div>
</template>

<style>

</style>