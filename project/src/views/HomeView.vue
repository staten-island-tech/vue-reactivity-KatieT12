<template>
  <div>
    <DestCard 
      v-for="product in products" 
      :key="product.name" 
      :Destination ="product"/>
      <!-- <ul>
        <li v-for="product in products" :key="product.name">
        {{ product.name }}
        <button @click="removeProduct(todo)>X</button>
        </li>
      </ul> -->
  </div>
</template>

<script setup>
import DestCard from "@/components/cartCards.vue";
//list of products added by button//
const products = [
      {
        name: "Porsche 911 GT3 RS",
        Used: false,
        price: 219797,
        img: "https://pictures.porsche.com/rtt/iris?COSY-EU-100-1711coMvsi60AAt5FwcmBEgA4qP8iBUDxPE3Cb9pNXABuN9dMGF4tl3U0%25z8rMHIspbWvanYb%255y%25XlvBCR8Z8CMj%25AH3kS6lm03mO1SZWjAgTbMtMdko5xjxiDLFC1aP2bsqYSghB0iO5MjAUHcTCkaToKfyUxFkprU9pNfqB0ubdMG0VPni2uFcLUB"
      }
    ]
</script>
<style scoped>
</style>