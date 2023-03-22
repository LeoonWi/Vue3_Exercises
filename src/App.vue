<script>
  export default {
    data() {
      return {
        msg: null,
        num: null,
      }
    },
    methods: {

    }
  }    
</script>

<template>
  <div>
    <input v-model="msg"><br>
    <p :style="{textTransform: 'uppercase'}">{{ msg }}</p>
  </div>
  <div>
    <input v-model="num"><br>
    <p>{{ num**2 }}</p>
  </div>
</template>

<style>

</style>