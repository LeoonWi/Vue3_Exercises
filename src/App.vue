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
            edit: false,
		    	},
		    	{
		    		id: 2,
		    		name: 'name2',
		    		salary: 200,
		    		age: 40,
            edit: false,
		    	},
		    	{
		    		id: 3,
		    		name: 'name3',
		    		salary: 300,
		    		age: 50,
            edit: false,
		    	},
		    ],
      };
    },
    methods: {
      delUser: function(id) {
        this.users = this.users.filter((user) => {
          return user.id != id;
        })
      },
      editUser: function(user) {
        user.edit = true;
      },
      saveUser: function(user) {
        user.edit = false;
      }
    }
  }    
</script>

<template>
  <table>
    <tr v-for="user in users" :key="user.id">
      <template v-if="!user.edit">
        <td>
          {{  user.name }}
        </td>
        <td>
          {{ user.salary }}
        </td>
        <td>
          {{ user.age }}
        </td>
      </template>
      <template v-if="user.edit">
        <td>
          <input type="text" v-model="user.name">
        </td>
        <td>
          <input type="text" v-model="user.salary">
        </td>
        <td>
          <input type="text" v-model="user.age">
        </td>
      </template>
      <td>
        <button @click="delUser(user.id)">Удалить пользователя</button>
      </td>
      <td>
        <button @click="editUser(user)" v-if="!user.edit">Редактировать пользователя</button>
        <button @click="saveUser(user)" v-if="user.edit">Сохранить пользователя</button>
      </td>
    </tr>
  </table>
</template>

<style>

</style>