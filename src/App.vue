<script>
  export default {
    data() {
      return {
        cssClasses: "red",
      }
    },
    methods: {
      
    }
  }    
</script>

<template>
  <p :class="cssClasses">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dignissimos, cum.</p>
</template>

<style>
.red {
  color: red;
}
</style>