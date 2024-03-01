<template>
    <div>
        <DestCard
        v-for="cartItems in cartItems"
        :key="cartItems.name"
        :product ="product"/>
       
    </div>

  </template>

  <script setup>
import DestCard from "@/components/cartCards.vue";
import { store} from '..stores/cart.js'


</script>
<style>
</style>