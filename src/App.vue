<script>
  export default {
    data() {
      return {
        arr: [],
        elem: 0,
      }
    },
    methods: {
      add: function() {
        this.arr.push(++this.elem);
      },
      del_start: function() {
        this.arr.shift();
      },
      del_pop: function() {
        this.arr.pop();
      },
      del_pre_last: function() {
        this.arr.splice(this.arr.length-2, 1);
      },
      sort: function() {
        this.arr.sort();
      },
      sort_rev: function() {
        this.arr.reverse();
      }
    }    
  }
</script>

<template>
  <div>
    <ul>
      <li v-for="elem in arr">{{ elem }}</li>
    </ul>    
  </div>
  <div>
    <button @click="add">Добавить в конце</button>
    <button @click="del_start">Удалить в начале</button>
    <button @click="del_pop">Удалить в конце</button>
    <button @click="del_pre_last">Удалить в предпоследний</button>
    <button @click="sort">Осортировать</button>
    <button @click="sort_rev">Осортировать в обратном порядке</button>
  </div>
</template>

<style>

</style>