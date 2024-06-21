<script setup>
import { ref, computed } from 'vue'

const counter = ref(0)

const squaredCounter = computed(() => counter.value ** 2)
// A computed property in Vue.js is a value that is automatically updated when one or more of its dependencies
// change. It is a cached value that is recalculated only when its dependencies change, making it efficient
// and useful for complex calculations or data transformations.

function incrementValue() {
    counter.value++

}

</script>

<template>
    <h1>{{ counter }}</h1>
    <h2>{{ squaredCounter }}</h2>
    <button @click="incrementValue">Increment</button>

</template>

<style scoped>
button {
    background-color: #4CAF50; /* Green */
    color: #fff;
    border-color: #4CAF50;
    padding: 10px 20px;
    border-radius: 5px;
  }

  button:hover {
    background-color: rgb(28, 120, 28);
    transition-duration: 3s;
    box-shadow: 0 8px 16px 0 rgba(136, 164, 91, 0.404), 0 12px 40px 0 rgba(99, 168, 113, 0.518);
  }

  button:active {
    background-color: #4CAF50; /* Green */
    color: #fff;
    border-color: #4CAF50;
    transform: scale(0.9); /* Scale down the button when clicked */
  }

</style>