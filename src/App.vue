<script>
  export default {
    data() {
      return {
        obj: {x: 2, y: 4, z: 6},
      }
    }
  }
</script>

<template>
  <div>
    <p>Сумма этих элементов: {{ obj.x + obj.y + obj.z }}</p>
  </div>
</template>

<style>

</style>