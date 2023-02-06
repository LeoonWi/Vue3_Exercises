<script>
  export default {
    data() {
      return {
        text: 'xxx',
      }
    },
    methods: {
      show: function() {
        this.text = 'xxx';
      },
      changeToY: function() {
        this.text = 'yyy';
      },
      changeToZ: function() {
        this.text = 'zzz';
      }
    }
  }
</script>

<template>
  <h1>{{ text }}</h1><br>
  <div>
    <button @click="changeToY">Превратить в Y</button><br>
    <button @click="changeToZ">Превратить в Z</button><br>
  </div>
  <div>
    <button @click="show">Сбросить</button>
  </div>
</template>

<style>

</style>