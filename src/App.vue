<script>
  export default {
    data() {
      return {
        items: [1, 2, 3],
      }
    },
    methods: {
      
    }    
  }
</script>

<template>
  <template v-for="elem in items">
    <div>
      <p>{{ elem }}</p>
      <p class="devider"></p>
    </div>
  </template>
  <div>
    <template v-for="elem in items">
      <ul>
        <li>{{ elem }}</li>
        <li class="devider"></li>
      </ul>
    </template>
  </div>
</template>

<style>

</style>