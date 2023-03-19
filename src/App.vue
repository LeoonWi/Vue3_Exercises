<script>
  export default {
    data() {
      let days = ['Воскресенье','Понедельник','Вторник','Среда','Четверг','Пятница','Суббота'];
      var d = new Date();
      var n = d.getDay();
      return {
        day: days[n],
      }
    },
    methods: {
      
    }    
  }
</script>

<template>
  <div>
    <p v-if="day === 'Воскресенье'">Воскресенье</p>
    <p v-if="day === 'Понедельник'">Понедельник</p>
    <p v-if="day === 'Вторник'">Вторник</p>
    <p v-if="day === 'Среда'">Среда</p>
    <p v-if="day === 'Четверг'">Четверг</p>
    <p v-if="day === 'Пятница'">Пятница</p>
    <p v-if="day === 'Суббота'">Суббота</p>
  </div>
</template>

<style>

</style>