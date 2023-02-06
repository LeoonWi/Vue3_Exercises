<script>
  export default {
    data() {
      return {
        visible: true,
      }
    },
    methods: {
      vis: function() {
        this.visible = true;
      },
      unvis: function() {
        this.visible = false;
      }
    }    
  }
</script>

<template>
  <div>
    <p v-if="visible">Первый абзац!</p>
    <p v-if="!visible">Второй абзац!</p>
  </div>
  <div>
    <button @click="vis" v-if="!visible">Показать первый абзац</button>
    <button @click="unvis" v-if="visible">Показать второй абзац</button>
  </div>
</template>

<style>

</style>