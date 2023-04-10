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
		func(name, salary) {
			alert(name + ' ' + salary);
		}
    }
  }    
</script>

<template>
  <Employer @show1="func"/>
</template>

<style>

</style>