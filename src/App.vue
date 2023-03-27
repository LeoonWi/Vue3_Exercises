<script>
  export default {
    data() {
      const today = new Date();
      const daysInMonth = new Date(today.getFullYear(), today.getMonth() + 1, 0).getDate();
      const daysArray = Array.from({ length: daysInMonth }, (_, i) => i + 1);
      const yearsArray = Array.from({ length: 10 }, (_, i) => today.getFullYear() - i);
      
      return {
        selectedDay: today.getDate(),
        selectedMonth: today.getMonth(),
        selectedYear: today.getFullYear(),
        days: daysArray,
        months: [
          "January",
          "February",
          "March",
          "April",
          "May",
          "June",
          "July",
          "August",
          "September",
          "October",
          "November",
          "December",
        ],
        years: yearsArray,
      };
    },
    methods: {
      
    }
  }    
</script>

<template>
   <div class="withMargin"> 
    <select v-model="selectedDay">
      <option v-for="day in days">{{ day }}</option>
    </select>
    <select v-model="selectedMonth">
      <option v-for="(month, index) in months" :key="index" :value="index">{{ month }}</option>
    </select>
    <select v-model="selectedYear">
      <option v-for="year in years">{{ year }}</option>
    </select>
  </div>
</template>

<style>

</style>