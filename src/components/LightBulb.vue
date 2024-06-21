<script setup>
import { ref } from "vue"

const isGlowing = ref(true)
const isShowing = ref(true)

const password = ref('123456789')

</script>

<template>
    <div style="margin-top: 20px;">
        <h1 v-show="isShowing">
            Click button to make me disappear 😎 !!
        </h1>
        <button @click="isShowing = !isShowing">Text toggle</button>
    </div>


    <div>
        <p v-if="isGlowing"><img src="https://i.postimg.cc/KjK1wL3c/bulb-off.png" alt="bulb not glowing"></p>
        <p v-else><img src="https://i.postimg.cc/6QyTynzr/bulb-on.png" alt="bulb glowing"></p>
        <button @click="isGlowing = !isGlowing">Toggle bulb on/off</button>
    </div>

</template>

<style>
img {
    width: 100px;
}
</style>
