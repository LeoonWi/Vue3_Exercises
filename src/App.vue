<script>
  export default {
    data() {
      return {
        age: 28,
      }
    },
    methods: {
      
    }    
  }
</script>

<template>
  <div>
    <p v-if="age < 18">Подросток</p>
    <p v-else-if="18 <= age && age < 25">Молодой</p>
    <p v-else-if="age >= 25">Зрелый</p>
  </div>
</template>

<style>

</style>