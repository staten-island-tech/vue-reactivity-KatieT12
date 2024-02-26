<script setup>
// import { RouterLink, RouterView } from 'vue-router'
</script>


<template>
  <header>
    <h1 class="title">Cars</h1>


      <nav>
        <RouterLink to="/products">Products</RouterLink>
        <!-- <RouterLink to="/">Cart</RouterLink> -->
      </nav>
      <div class="listing">
      <Router-view />
      </div>


    <div class="container">
      <h1 class="cartTitle">Cart</h1>
      <div class="itemsinCart"></div>
      <button class="checkOutbtn">Check Out</button>
    </div>
  </header>


</template>


<style scoped>
.container{
  background-color: rgb(255, 255, 255);
  color: #044B7F;
  width: 20%; height: 100%;
  float: right;
  position: absolute;
  top: 10rem;
  right: 2rem;
  overflow: scroll;
  overflow-y: auto;
  border: black;
  border-radius: 3rem;
  border-color: black;
  display: flex;
  align-items: center;
  flex-direction: column;
  border-style: solid;
  border-color: #044B7F;
}
.title, .cartTitle, nav{
  text-align: center;
}
.checkOutbtn{
  background-color: #044B7F;
  color: white;
  border-radius: 1rem;
  margin-top: 3rem;
  width: 20rem; height: 50px;
  font-size: 1.5rem;
  margin-bottom: 3rem;
}
.itemsinCart{
display: flex;
flex-direction: column;
align-items: center;
}
/* .listing{
    display: flex;
    width: 90%;
    flex-wrap: wrap;
    justify-content: space-around;
    margin: 5rem auto;
    padding: 5px;
    flex-direction: row;
} */


</style>
