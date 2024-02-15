<template>
  <div>
      <DestCard 
      v-for="destination in destinations" 
      :key="destination.name" 
      :Destination ="destination"/>
      <button></button>
  </div>
</template>

<script setup>
import DestCard from "@/components/DestCard.vue";


</script>
<style scoped>
/* @media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
} */
</style>