<script>
  import Employer from './components/Employee.vue'
  
  export default {
    components: {
      Employer
    },
    data() {
      return {
        name: 'Данил',
        surname: 'Ромашкан',
        age: 18
      };
    },
    methods: {
      
    }
  }    
</script>

<template>
  <Employer :name="name" :surname="surname" :age="age"/>
</template>

<style>

</style>