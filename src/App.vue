<script>
  export default {
    data() {
      return {
        isValid: true,
	    	isDisabled: false,
      }
    },
    methods: {
      
    }
  }    
</script>

<template>
  <p :class="{active: isValid, inactive: isDisabled}">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dignissimos, cum.</p>
</template>

<style>
  p.active {
  	text-decoration: underline;
  }
  p.inactive {
    display: none;
  }
</style>