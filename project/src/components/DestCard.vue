<template>
    <div>
        <h2>{{ name }}</h2>
        <h3>${{ price }}</h3>
        <img :src="img" alt="insert image here"/>
        <h3>{{ clicked }}</h3>
        <button @click="increment">Click Me</button>
    </div>
</template>

<script setup>
import {ref, defineProps} from "vue";
defineProps({
    name: String,
    img: String,
    price: Number,
});

//clicker logic
const clicked = ref(0);
function increment(){
    clicked.value++
}
</script>

<style scoped>
img{
    width: 250px;
    height: 300px;
    object-fit: cover;
}
</style>