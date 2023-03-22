<script>
  export default {
    data() {
      return {
        text: null,
        text2: '',
        arr: [],
      }
    },
    methods: {
      sep: function() {
        this.arr = this.text2.split(',');
      }
    }
  }    
</script>

<template>
  <div>
    <p>{{ text }}</p>
    <textarea v-model="text" cols="30" rows="10" placeholder="Введите текст"></textarea>
  </div>
  <div>
    <textarea v-model="text2" cols="30" rows="10" placeholder="Введите что-нибудь"></textarea><br>
    <button @click="sep">Отправить</button><br>
    <ul>
      <li v-for="elem in arr">{{ elem }}</li>
    </ul>
  </div>
</template>

<style>

</style>