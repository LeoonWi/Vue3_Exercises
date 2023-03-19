<script>
  export default {
    data() {
      return {
        vis_one: true,
        vis_two: true,
        vis_three: true
      }
    },
    methods: {
      first: function() {
        this.vis_one = !this.vis_one;
      },
      second: function() {
        this.vis_two = !this.vis_two;
      },
      third: function() {
        this.vis_three = !this.vis_three;
      }
    }    
  }
</script>

<template>
  <div>
    <p v-if="vis_one">Первый абзац!</p>
    <p v-if="vis_two">Второй абзац!</p>
    <p v-if="vis_three">Третий абзац!</p>
  </div>
  <div>
    <button @click="first">{{ vis_one ? 'Скрыть' : 'Показать'}} первый абзац</button>
    <button @click="second">{{ vis_two ? 'Скрыть' : 'Показать'}} второй абзац</button>
    <button @click="third">{{ vis_three ? 'Скрыть' : 'Показать'}} третий абзац</button>
  </div>
</template>

<style>

</style>