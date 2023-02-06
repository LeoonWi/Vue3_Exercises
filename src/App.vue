<script>
  export default {
    data() {
      return {
        num: '',
      }
    },
    methods: {
      show: function(str) {
        if (str == 'sqr') alert(Math.pow(this.num, 2));
        else if (str == 'pwr3') alert(Math.pow(this.num, 3));
      }
    }
  }
</script>

<template>
  <div>
    Введите число:<br>
    <input type="text" v-model="num">
  </div><br>
  <button @click="show('sqr')">Возвести в квадрат</button><br>
  <button @click="show('pwr3')">Возвести в третью степень</button>
</template>

<style>

</style>