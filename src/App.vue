<script>
  export default {
    data() {
      return {
        items: [1, 2, 3, 4, 5],
      }
    },
    methods: {
      
    }    
  }
</script>

<template>
  <div>
    <div v-for="n in items">{{ n }}</div>
  </div>
  <div>
    <div v-for="n in items">{{ n**2 }}</div>
  </div>
  <div>
    <ul><li v-for="n in items">{{ n }}</li></ul>
  </div>
</template>

<style>

</style>