<script>
  export default {
    data() {
      return {
        hrefs: [
		    	{href: '1.html', text: 'text1'},
		    	{href: '2.html', text: 'text2'},
		    	{href: '3.html', text: 'text3'},
		    ],
        products: [
		    	{
		    		name: 'product1',
		    		price: 100,
		    		quantity: 5
		    	},
		    	{
		    		name: 'product2',
		    		price: 200,
		    		quantity: 4
		    	},
		    	{
		    		name: 'product3',
		    		price: 300,
		    		quantity: 3
		    	}
        ],
      }
    },
    methods: {
      
    }    
  }
</script>

<template>
  <div>
    <ul>
      <template v-for="elem in hrefs">
        <li><a v-bind:href="elem.href">{{ elem.text }}</a></li>
      </template>
    </ul>    
  </div>
  <div>
    <table>
      <template v-for="elem in products">
        <td>
          <tr>{{ elem.name }}</tr>
          <tr>{{ elem.price }}</tr>
          <tr>{{ elem.quantity }}</tr>
        </td>
      </template>
    </table>
  </div>
 </template>

<style>

</style>