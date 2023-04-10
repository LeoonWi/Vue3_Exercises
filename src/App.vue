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
		Name() {
            alert('Данил');
        },
        Salary() {
            alert('10000');
        },
    }
  }    
</script>

<template>
  <Employer @show1="Name" @show2="Salary"/>
</template>

<style>

</style>