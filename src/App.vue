<script>
  export default {
    data() {
      return {
        arr: ['3', '5', '7']
      }
    }
  }
</script>

<template>
  <div>
    <p>Первый элемент: {{ arr[0] }}</p>
    <p>Второй элемент: {{ arr[1] }}</p>
    <p>Третий элемент: {{ arr[2] }}</p>
  </div>
  <div>
    <p>Сумма этих элементов: {{ arr[0] + arr[1] + arr[2] }}</p>
  </div>
</template>

<style>

</style>