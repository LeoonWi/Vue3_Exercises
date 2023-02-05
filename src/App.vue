<script>
  export default {
    data() {
      return {
        num1: 10,
        num2: 15,
        num3: 20,
      }
    }
  }
</script>

<template>
  <div>
    <h1>Возведение {{ num1 }} в степень: {{ Math.pow(num1,2) }}</h1>
    <h1>Сумма: {{ num1 }} + {{ num2 }} + {{ num3 }} = {{ num1 + num2 + num3 }}</h1>
  </div>
</template>

<style>

</style>