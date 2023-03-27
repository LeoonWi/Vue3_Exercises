<script>
  export default {
    data() {
      return {
        city: null,
      }
    },
    methods: {
      
    }
  }    
</script>

<template>
  <p>В каком городе вы живёте?</p><br>
  <select v-model="city">
    <option>Симферополь</option>
    <option>Лондон</option>
    <option>Матрица</option>
  </select><br>
  <p>{{ city }}</p>
</template>

<style>

</style>