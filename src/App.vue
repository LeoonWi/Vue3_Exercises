<script>
  import Employer from './components/Employee.vue'
  
  export default {
    components: {
      Employer
    },
    data() {
      return {
        
      };
    },
    methods: {
      
    }
  }    
</script>

<template>
  <Employer :arr="[1, 2, 3, 4]"/>
</template>

<style>

</style>