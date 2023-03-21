<script>
  export default {
    data() {
      return {
        obj: {
          red: true,
          dashed: false
        },
      }
    },
    methods: {
      
    }
  }    
</script>

<template>
  <p :class="obj">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dignissimos, cum.</p>
</template>

<style>
.red {
  color: red;
}
.dashed {
  text-decoration: underline;
}
</style>