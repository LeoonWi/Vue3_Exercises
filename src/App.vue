<script>
  export default {
    data() {
      return {
        obj: {
	        user1: '100$',
	        user2: '200$',
	        user3: '300$',
        },
      }
    },
    methods: {
      
    }    
  }
</script>

<template>
  <div>
    <ul><li v-for="(n, k, i) in obj">{{ n }}</li></ul>
    <ul><li v-for="(n, k, i) in obj">{{ k }} - {{ n }}</li></ul>
    <ul><li v-for="(n, k, i) in obj">{{ k }} - {{ n }} - {{ i+1 }}</li></ul>
  </div>
</template>

<style>

</style>