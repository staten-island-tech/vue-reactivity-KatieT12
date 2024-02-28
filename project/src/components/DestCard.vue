<template>
    <div>
        <h2>{{ product.name }}</h2>
        <img :src="product.img" alt=""/>
        <h3> Price: {{ product.price }}</h3>
        <button @click="addtoCart">Add to Cart</button>

        <form @submit.prevent="addTodo">
    <input v-model="newTodo" required placeholder="new todo">
    <button>Add Todo</button>
  </form>
  <ul>
    <li v-for="todo in todos" :key="todo.id">
      {{ todo.text }}
      <button @click="removeTodo(todo)">X</button>
    </li>
  </ul>
  
    </div>
</template>


<script setup>
import {ref} from "vue";
const props = defineProps({
    product: Object,
});
// give each todo a unique id
let id = 0

const newTodo = ref('')
const todos = ref([
  { id: id++, text: 'Learn HTML' },
  { id: id++, text: 'Learn JavaScript' },
  { id: id++, text: 'Learn Vue' }
])

function addtoCart() {
  todos.value.push({ id: id++, text: newTodo.value })
  newTodo.value = ''
}

function removefromCart(todo) {
  todos.value = todos.value.filter((t) => t !== todo)
}



// const DOMSelectors = {
//     container: document.querySelector(".container"),
//     removebuttons: document.querySelectorAll(".Remove"),
//     cartContent: document.querySelector(".itemsinCart"),
    
// }
// function addtoCart(){
//      DOMSelectors.cartContent.insertAdjacentHTML(
//        "beforeend",
//         `<div class = "card">
//         <h3 class="name">Name: ${props.name}</h3>
//         <img src=${props.img}> </img>
//         <h4 class="price">Price: ${props.price}</h4>
//         <button type ="button" class="Remove" @click="removeItem">Remove Item</button>
//         <br>
//     </div>`
//      );
// };

// function removeItem(){
//     let removebuttons = document.querySelectorAll(".Remove")
//     removebuttons.forEach((element) => element.addEventListener('click', function(){
//     element.parentElement.remove();
//             }));
//          };
// removeItem();


</script>

<style scoped>
img{
    width: 20%;
    height: 100%;
    object-fit: cover;
}
button{
background-color: #0073ff;
color: white;
border-radius: 1rem;
width: 20rem; height: 50px;
font-size: 1.5rem;
margin-bottom: 3rem;
}
.Remove{ /*not working */
background-color: #0073ff;
  color: white;
  border-radius: 1rem;
  margin-top: 3rem;
  width: 20rem; height: 50px;
  font-size: 1.5rem;
  margin-bottom: 3rem;
}

</style>