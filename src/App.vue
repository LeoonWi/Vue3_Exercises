<script>
  export default {
    data() {
      return {
        users: [
		    	{
		    		id: 1,
		    		name: 'name1',
		    		salary: 100,
		    		age: 30,
		    	},
		    	{
		    		id: 2,
		    		name: 'name2',
		    		salary: 200,
		    		age: 40,
		    	},
		    	{
		    		id: 3,
		    		name: 'name3',
		    		salary: 300,
		    		age: 50,
		    	},
		    ],
      };
    },
    methods: {
      delUser: function(id) {
        this.users = this.users.filter((user) => {
          return user.id != id;
        })
      }
    }
  }    
</script>

<template>
  <table>
    <tr v-for="user in users" :key="user.id">
      <td>
        {{  user.name }}
      </td>
      <td>
        {{ user.salary }}
      </td>
      <td>
        {{ user.age }}
      </td>
      <td>
        <button @click="delUser(user.id)">Удалить пользователя</button>
      </td>
    </tr>
  </table>
</template>

<style>

</style>