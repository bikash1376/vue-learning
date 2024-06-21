<script setup>
import { reactive, ref } from 'vue';

const title = ref("Hello World")       
// ref is used for single value
const list = reactive([ref("Bikash"), ref("20"), ref("Jamshedpur")])
// reactive is used for multiple values like for arrays and objects

</script>


<template>
    <h1> {{ title }} </h1>
    <button @click="title = 'Hello peeps'" class="blue-btn">Change</button>
    <h1>{{ list }}</h1>
    <button  @click="list[0] = 'Rohan', list[1] = '29', list[2] = 'Bangalore'"  class="blue-btn">Change List</button>
</template>

<style>
* {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: black;
    color: white;
}

button {
    border: none;
    padding: 10px 20px;
    background-color: blue;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: rgb(35, 35, 170);
    transition-duration: 1s;
    box-shadow: 0 8px 16px 0 rgba(91, 91, 164, 0.244), 0 12px 40px 0 rgba(99, 99, 168, 0.418);
}
button:active {
    background-color: #4CAF50; /* Green */
    color: #fff;
    border-color: #4CAF50;
    transform: scale(0.9); /* Scale down the button when clicked */
  }
</style>
