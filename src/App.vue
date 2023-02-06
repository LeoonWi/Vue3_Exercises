<script>
  export default {
    data() {
      return {
        name: 'Фисташки',
        cost: '50',
        amount: '1500',
      }
    },
    methods: {
      
    },
    computed: {
      price: function() {
        return this.cost * this.amount;
      }
    }
  }
</script>

<template>
  <div>
    <p>{{ name }}: {{ amount }} шт. {{ cost }} руб./шт.</p>
    <p>Итого: {{ price }} руб.</p><br>
  </div>
  <div>
    Введите новую цену: <input type="text" v-model="cost">
  </div>
</template>

<style>

</style>