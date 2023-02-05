<script>
  export default {
    data() {
      return {
        name: 'page',
        href: '../page.html'
      }
    }
  }
</script>

<template>
  <div>
    <a :href="href">{{ name }}</a> <!-- для работы с атрибутами, нужно юзать v-bind:свойство или :свойство -->
  </div>
</template>

<style>

</style>