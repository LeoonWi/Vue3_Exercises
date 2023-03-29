<script>
  export default {
    data() {
      return {
        arr: [],
        message: '',
      };
    },
    methods: {
      addElem: function() {
        this.arr.push(this.message)
      },
      addElemToStart: function() {
        this.arr.unshift(this.message)
      }
    }
  }    
</script>

<template>
    <input type="text" v-model="message"><br>
    <button @click="addElemToStart">Добавить новый элемен в начало</button><br>
    <button @click="addElem">Добавить новый элемен в конец</button>
    <ul>
      <li v-for="(elem, index) in arr" :key="index">{{ elem }}</li>
    </ul>
</template>

<style>

</style>