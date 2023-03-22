<script>
  export default {
    data() {
      return {
        arr: [],
      }
    },
    methods: {
      
    }
  }    
</script>

<template>
  <p>Какие языки вы знаете?</p><br>
  <div>
    <label><input type="checkbox" v-model="arr" value="Английский"> Английский</label><br>
    <label><input type="checkbox" v-model="arr" value="Французский"> Французский</label><br>
    <label><input type="checkbox" v-model="arr" value="Русский"> Русский</label><br>
  </div>
  <ul>
    <li v-for="elem in arr">{{ elem }}</li>
  </ul>
</template>

<style>

</style>