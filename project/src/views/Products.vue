<template>
  <div>
      <DestCard
      v-for="product in products"
      :key="product.name"
      :product ="product"/>
  </div>
</template>


<script setup>
import DestCard from "@/components/DestCard.vue";
const products = [
      {
        name: "Porsche Panamera 4",
        price: 108970,
        img: "https://pictures.porsche.com/rtt/iris?COSY-EU-100-1711coMvsi60AAt5FwcmBEgA4qP8iBUDxPE3Cb9pNXABuN9dMGF4tl3U0%25z8rMHIspMBvMZq6G5OtgSv31nBJaA4qh4NSEGkaW%25cz91wxuzbUUdMGLqk0D34oQDcFGjiuWXsOYA9eV6iTmCCzhRc2gEcqA7fQlOGOJUPYJvCTBsN5BxG2dioCdqoQDcFGH6zYnfuroA65yPewF%25oCvNzxu0EGXoq1quRr6FObOhswRuT0Tpzx7e2HRiO1UzQKmVZbsqYSgfV0iO5M4dCvNzxKjYGXoq1SCzr6FObUZ9wRAyYib32yl3UIqGKaYW1TG87hXuci601"
      },
      {
        name: "Porsche Cayenne",
        price: 85880,
        img: "https://pictures.porsche.com/rtt/iris?COSY-EU-100-1711coMvsi60AAt5FwcmBEgA4qP8iBUDxPE3Cb9pNXABuN9dMGF4tl3U0%25z8rMHIspMBvMZq6G5OtgSv31nBJaA4qh4NSEGkaW%25cz91wxuzbUUdMGLqk0D34tQDcFGDANYnfurn0x5yPewy2eCvNzxzmJGXoq1nDrr6FObNCTBsN5xlz2dioC16F%25vUqYhQuWXsOASIeV6iTJX8zhp4NdTxf4KxJhMuYoNmOcuLAlWRDdV2Tr"
      },
      {
        name: "Porsche Macan 4 Electric",
        price: 82880,
        img: "https://pictures.porsche.com/rtt/iris?COSY-EU-100-1711coMvsi60AAt5FwcmBEgA4qP8iBUDxPE3Cb9pNXABuN9dMGF4tl3U0%25z8rMHIspMBvMZq6G5OtgSv31nBJaA4qh4NSEGkaW%25cz91wxuzbUUdMGLqk0D3LEQDcFGIoBYnfur3eN5yPewjloCvNzxa07GXoq1%25SSr6FOb6cHwRuT0RAMx7e2H7nS1UzQKjFlbsqYS29Y0iO5MQ6BHcTCkYvGXoq1eH9r6FObOW0wRuT0Tyqx7e2H2qs1UzQKQtObsqYSRpP0iO5Mo6YHcTCkpJTKf2GLe%25GSPQrIH8wRuT0k%25Ax7e2HLPn1UzQKIx2bsqYS5wI0iO5MP4hHcTCkNO6KfyUxFkprU9pN55KaExdMG0VPni2uFcLM"
      },
      {
        name: "Porsche Taycan",
        price: 108375,
        img: "https://pictures.porsche.com/rtt/iris?COSY-EU-100-1711coMvsi60AAt5FwcmBEgA4qP8iBUDxPE3Cb9pNXkBuNYdMGF4tl3U0%25z8rMHIspMBvMZq6G5OtgSv31nBJaA4qh4NSEGkaW%25cz91wxuzbUUdMGLqk0D3LEQDcFGImPYnfurEFu5yPew9AeCvNzxvCWGXoq1XS0r6FOb6tjwRuT0Rxrx7e2H7G21UzQKTvfbsqYS2dT0iO5MQIAHcTCkCdLKf2GLGU5SPQrIr5oMNYw3wWCko5xjNerLFC1aOcxIuGbm5L0iO5MlAkHcTCkBOoKf2GLeEHSPQrIKOwRuT0rFTx7e2HLWJ1UzQKIx2bsqYS3zJ0iO5MP4hHcn7woMlG7ElPgBbIxwBSCbWfDsTFoik4"
      },
      {
        name: "Rivian R1T",
        price: 71650,
        img: "https://media.rivian.com/rivian-main/c_fill,w_1920/q_auto,f_auto/compositor/r1t/front/2023.1,bat-c01,exp-fgr,int-bmp,mot-201,ord-ad3,pkg-adv,rgn-usa,whl-1rd,studio"
      },
      {
        name: "Rivian R1S",
        price: 99100,
        img: "https://media.rivian.com/rivian-main/c_fill,w_1920/q_auto,f_auto/compositor/r1s/front/2023.1,atp-001,bat-b01,exp-mdn,int-bmp,mot-401,ord-ad2,ord-ad3,pkg-adv,rgn-usa,swh-cst,whl-0ad,studio"
      },
    ]


</script>
<style>

</style>