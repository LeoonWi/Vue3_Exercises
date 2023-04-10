<script>
    export default {
        props: {
            id: Number,
            name: String,
            surn: String
        },
        emits: ['remove', 'change'],
        data() {
            return {
                Edit: false,
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
        }
    }
</script>

<template>
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