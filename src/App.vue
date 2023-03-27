<script>
  export default {
    data() {
      return {
        lang: null,
      }
    },
    methods: {
      
    }
  }    
</script>

<template>
  <p>Выберите язык</p><br>
  <div>
    <label><input type="radio" name="lang" v-model="lang" value="ru"> Русский</label><br>
    <label><input type="radio" name="lang" v-model="lang" value="eng"> Английский</label><br>
    <label><input type="radio" name="lang" v-model="lang" value="bin"> Машинный язык</label>
  </div><br>
  <p v-if="lang === 'ru'">Привет!</p>
  <p v-if="lang === 'eng'">Hello!</p>
  <p v-if="lang === 'bin'">0x55 0x89 0xe5 0xe8 0xfc 0xff 0xff 0xff 0x83 0xf8 0x41 0x75 0x0d 0x68 0x00 0x00 0x00 0x00 0xe8 0xfc 0xff 0xff 0xff 0x83 0xc4 0x04 0xb8 0x00 0x00 0x00 0x00 0x89 0xec 0x5d 0xc3</p>
  
</template>

<style>

</style>