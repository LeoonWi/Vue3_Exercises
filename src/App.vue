<script>
  export default {
    data() {
      return {
        num_day: null,
      }
    },
    methods: {
      show: function() {
        let date = new Date();
        let Day = date.getDay();
        let weekDay = ['Воскресенье', 'Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота'];
        alert(weekDay[Day]);
      },
      now_day: function() {
      
        return weekDay[nDay];
      },
      numday: function() {
        let Num_Day = this.day(this.num_day);
        alert(Num_Day);
      },
      day: function(nDay) {
        let weekDay = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота' ,'Воскресенье'];
        return weekDay[nDay-1];
      }
    }
  }
</script>

<template>
  <form action="" @submit="numday">
    Введите номер недели:<br>
    <input type="number" v-model="num_day" name="numday" min="1" max="7">
    <button type="submit">Нажми на меня</button>
  </form><br>
  <button @click="show">Показать текущий день недели</button>
</template>

<style>

</style>