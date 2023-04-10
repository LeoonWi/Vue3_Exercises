<script>
  import Employer from './components/Employee.vue'
  
  export default {
    components: {
      	Employer
    },
    data() {
      	return {
			users: [
				{
					id: 1,
					name: 'name1',
					surn: 'surn1'
				},
				{
					id: 2,
					name: 'name2',
					surn: 'surn2'
				},
				{
					id: 3,
					name: 'name3',
					surn: 'surn3'
				},
			],
      	};
    },
    methods: {
		remove(id) {
			this.users = this.users.filter((user) => {
				return user.id !== id;
			})
		},
		change(id, name, surn) {
			this.users = this.users.map((user) => {
				if (user.id === id) {
					user.name = name;
					user.surn = surn;
				}
				return user;
			});
		},
		add(name, surn) {
			let id = this.users.length + 1;
			
			this.users.push({
				id,
				name,
				surn
			});
		}	
    }
  }    
</script>

<template>
  <Employer v-for = "user in users"
	:id = "user.id"
	:name = "user.name"
	:surn = "user.surn"
	@remove = "remove"
	@change = "change"
	@add = "add"
	:key = "user.id"/>
</template>

<style>

</style>