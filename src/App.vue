<script>
  export default {
    data() {
      return {
        count: 0,
      }
    },
    methods: {
      once: function() {
        return this.count++;
      }
    }    
  }
</script>

<template>
  <a href="https://youtube.com" @click.prevent>Youtube.com</a><br>
  <button @click.once="once">Приветствие №{{ count }}</button>
</template>

<style>

</style>