<template>
    <div>
        <h2>{{ Destination.name }}</h2>
        <img :src="Destination.img" alt=""/>
        <h3>Number Currently in Cart: {{ clicked }}</h3>
        <button @click="addtoCart">Add to Cart</button>
    </div>
</template>


<script setup>
import {ref} from "vue";


const props = defineProps({
    Destination: Object,
});


//clicker logic
// const clicked = ref(0);
// function increment(){
//     clicked.value++
// }
const DOMSelectors = {
    container: document.querySelector(".container"),
    removebuttons: document.querySelectorAll(".Remove"),
    cartContent: document.querySelector(".itemsinCart")
}
const clicked= ref(0)
function addtoCart(){
    clicked.value++
     DOMSelectors.cartContent.insertAdjacentHTML(
       "beforeend",
        `<div class = "card">
        <h3 class="name">Name: ${props.name}</h3>
        <h4 class="used">Used: ${props.Used}</h4>
        <img src=${props.img}> </img>
        <h4 class="price">Price: ${props.price}</h4>
        <button type ="button" class="Remove">Remove Item</button>
        <br>
    </div>`
     );
};


function removeItem(){
    let removebuttons = document.querySelectorAll(".Remove")
    removebuttons.forEach((element) => element.addEventListener('click', function(){
    element.parentElement.remove();
            }));
         };
</script>


<style scoped>
img{
    width: 20%;
    height: 100%;
    object-fit: cover;
}
.Remove{
    margin-bottom: 100rem;
}
</style>