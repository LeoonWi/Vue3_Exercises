<script>
    export default {
        props: {
            id: Number,
            name: String,
            surn: String
        },
        emits: ['remove', 'change', 'add'],
        data() {
            return {
                Edit: false,
                Add: false,
                newName: this.name,
                newSurn: this.surn,
            };
        },
        methods: {
            isEdit() {
                this.Edit = true;
            },
            isSave() {
                this.Edit = false;
                this.$emit('change', this.id, this.newName, this.newSurn);
            },
            isAdd() {
                this.Add = true;
            },
            save() {
                this.Add = false;
                this.$emit('add', this.newName, this.newSurn);
            }
        }
    }
</script>

<template>
    <button @click="isAdd" v-if="!Add">Добавить пользователя</button><br>
    <template v-if="Add">
        <label for="">Имя <input v-model="newName"></label><br>
	    <label for="">Фамилия <input v-model="newSurn"></label><br>
        <button @click="save">Сохранить пользователя</button><br>
    </template>
    <template v-if="!Edit">
        <p>{{ name }} {{ surn }}</p><br>
        <button @click="$emit('remove', id)">Удалить</button><br>
        <button @click="isEdit">Редактировать</button><br>
    </template>
    <template v-if="Edit">
        <p><input v-model="newName"> <input v-model="newSurn"></p><br>
        <button @click="isSave">Сохранить</button>
    </template>
</template>