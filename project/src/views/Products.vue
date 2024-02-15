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
const destinations = [
      {
        name: "2015 Volkswagen Beetle",
        Used: true,
        price: 18998,
        img: "https://img2.carmax.com/assets/25099732/hero.jpg?width=800&height=450"
      },
      {
        name: "2017 Fiat 500",
        Used: true,
        price: 14995,
        img: "https://www.motortrend.com/uploads/sites/10/2016/12/2017-fiat-500-pop-hatchback-angular-front.png?fit=around%7C875:492"
      },
      {
        name: "2016 Mazda MX-5 Miata Grand Touring",
        Used: true,
        price: 21998,
        img: "https://img2.carmax.com/assets/25052772/hero.jpg?width=800&height=450"
      },
      {
        name: "2023 Lexus RZ450E",
        Used: false,
        price: 900,
        img: "https://www.longolexus.com/static/group-longo-group/2023-lexus-rz/2023-lexus-rz.png"
      },
      {
        name: "2016 Nissan GT-R",
        Used: false,
        price: 400,
        img: "https://www.motortrend.com/uploads/sites/10/2015/11/2016-nissan-gtr-premium-coupe-angular-front.png"
      },
      {
        name: "Porsche 911 GT3 RS",
        Used: false,
        price: 219797,
        img: "https://pictures.porsche.com/rtt/iris?COSY-EU-100-1711coMvsi60AAt5FwcmBEgA4qP8iBUDxPE3Cb9pNXABuN9dMGF4tl3U0%25z8rMHIspbWvanYb%255y%25XlvBCR8Z8CMj%25AH3kS6lm03mO1SZWjAgTbMtMdko5xjxiDLFC1aP2bsqYSghB0iO5MjAUHcTCkaToKfyUxFkprU9pNfqB0ubdMG0VPni2uFcLUB"
      },
    ]

</script>
<style>
@media (min-width: 1024px) {
  .products {
    min-height: 100vh;
    display: flex;
    /* align-items: row; */
  }
}
</style>
