<script>
  export default {
    data() {
      return {
        vis: true,
      }
    },
    methods: {
      visible: function() {
        this.vis = !this.vis;
      }
    }    
  }
</script>

<template>
  <div v-if="vis">
    <p>1 абзац</p>
    <p>2 абзац</p>
    <p>3 абзац</p>
  </div>
  <button @click="visible">{{ vis ? 'Показать':'Скрыть' }} абзацы</button>
</template>

<style>

</style>