<script>
  export default {
    data() {
      return {
        checked: true,
      }
    },
    methods: {
      
    }
  }    
</script>

<template>
  <input type="checkbox" v-model="checked">
  <p v-if="checked">Чёт написано</p>
</template>

<style>

</style>