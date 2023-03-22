<script>
  export default {
    data() {
      return {
        num: 0,
        res1: 0,
        num1: 0,
        num2: 0,
        txt1: '',
        txt2: '',
        fio: '',
        arr: [],
      }
    },
    methods: {
      sqr: function() {
        this.res1 = this.num**2;
      },
      sum: function() {
        this.res2 = this.num1 + this.num2;
      },
      txt: function() {
        let temp = this.txt1;
        this.txt1 = this.txt2;
        this.txt2 = temp;
      },
      sep: function() {
        this.arr = this.fio.split(' ');
      }
    }
  }    
</script>

<template>
  <div>
    <input v-model="num">
    <button @click="sqr">Отправить</button><br>
    <p>Ответ: {{ res1 }}</p>
  </div>
  <div>
    <input v-model="num1">
    <input v-model="num2">
    <button @click="sqr">Отправить</button><br>
    <p>Ответ: {{ res2 }}</p>
  </div>
  <div>
    <input v-model="txt1">
    <input v-model="txt2">
    <button @click="txt">Отправить</button><br>
    <p>Ответ: {{ txt1 }} и {{ txt2 }}</p>
  </div>
  <div>
    <input v-model="fio">
    <button @click="sep">Отправить</button><br>
    <p>Ответ: {{ arr[0] }}</p>
    <p>Ответ: {{ arr[1] }}</p>
    <p>Ответ: {{ arr[2] }}</p>
  </div>
</template>

<style>

</style>