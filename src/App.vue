<script>
  export default {
    data() {
      return {
        obj: {
		    	hidden: true,
		    },
      }
    },
    methods: {
      hide: function() {
        this.obj.hidden = !this.obj.hidden;
      }
    }
  }    
</script>

<template>
  <p :class="obj">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dignissimos, cum.</p>
  <button @click="hide">Спрятать/Отобразить</button>
</template>

<style>
  p.hidden {
  	display: none;
  }
</style>