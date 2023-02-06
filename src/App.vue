<script>
  export default {
    data() {
      return {
        num1: 5,
        num2: 10,
      }
    },
    methods: {
      show: function() {
        alert(this.num1 + this.num2);
      }
    }
  }
</script>

<template>
  {{ show() }}
</template>

<style>

</style>