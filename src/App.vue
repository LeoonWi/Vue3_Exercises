<script>
  export default {
    data() {
      return {
        isAdmin: true,
      }
    },
    methods: {
      
    }    
  }
</script>

<template>
  <div>
    <p v-if="isAdmin">Админ</p>
    <p v-else>Пользователь</p>
  </div>
</template>

<style>

</style>