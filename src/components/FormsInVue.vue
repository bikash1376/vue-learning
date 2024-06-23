<script setup>
import { reactive, ref } from 'vue';
const formData = ref({
    username: '',
    email: '',
    password: ''

})
</script>

<template>
    <form @submit.prevent>
    <input type="text" placeholder="Enter username" v-model="formData.username">
    <input type="email" placeholder="Enter email" v-model="formData.email">
    <input type="password" placeholder="Enter password" v-model="formData.password">
    <button type="submit">Submit</button>
    </form>

    <div>
    <li>{{ formData.username }}</li>
    <li>{{ formData.email }}</li>
    <li>{{ formData.password }}</li>
    </div>
</template>

<style>
form {
    font-size: 30px;
}
input {
    font-size: 20px;
    padding: 10px 20px;
}
</style>