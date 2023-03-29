<script>
  export default {
    data() {
      return {
        isDisable: false,
      };
    },
    methods: {
      disable: function() {
        this.isDisable = !this.isDisable
      }
    }
  }    
</script>

<template>
    <input type="checkbox" @click="disable">
    <input v-bind:disabled="isDisable" type="text">
</template>

<style>

</style>