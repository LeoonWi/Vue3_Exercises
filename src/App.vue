<script>
  export default {
    data() {

    },
    methods: {
      show: function() {
        alert(Date());
      }
    }
  }
</script>

<template>
  <div>
    <button v-on:click="show">Текущая дата кликом</button>
  </div>
  <div> <!-- Обраб. события вызываемся v-on: либо @ -->
    <button @mouseover="show">Текущая дата наведением</button>
  </div>
</template>

<style>

</style>