<template>
    <div>
        <h2>{{ Destination.name }}</h2>
        <img :src="Destination.img" alt=""/>
        <h3>Number Currently in Cart: {{ clicked }}</h3>
        <button @click="increment">Add to Cart</button>
    </div>
</template>

<script setup>
import {ref} from "vue";
const props = defineProps({
    Destination: Object,
});

//clicker logic
const clicked = ref(0);
function increment(){
    clicked.value++
}
</script>

<style scoped>
img{
    width: 20%;
    height: 100%;
    object-fit: cover;
}
</style>