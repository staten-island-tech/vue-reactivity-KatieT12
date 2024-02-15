<template>
    <div>
        <h2>{{ Product.name }}</h2>
        <img :src="Product.img" alt=""/>
        <h3>Number Currently in Cart: {{ clicked }}</h3>
        <button @click="removefromCart">Remove From Cart</button>
    </div>
</template>

<script setup>
import {ref} from "vue";

const props = defineProps({
    Product: Object,
});

//clicker logic
// const clicked = ref(0);
// function increment(){
//     clicked.value++
// }

const clicked= ref(0)
function removefromCart(){
    clicked.value--
}
</script>

<style scoped>
img{
    width: 20%;
    height: 100%;
    object-fit: cover;
}
</style>