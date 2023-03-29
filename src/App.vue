<script>
  export default {
    data() {
      return {
        arr: [1, 2, 3, 4, 5, 6, 7, 8, 9, 0],
        message: '',
      };
    },
    methods: {
      delElem: function(index) {
        this.arr.splice(index, 1)
      }
    }
  }    
</script>

<template>
    <button @click="delElem(index)">Удалить элемент</button><br>
    <ul>
      <li v-for="(elem, index) in arr" :key="index">{{ elem }}</li>
    </ul>
</template>

<style>

</style>