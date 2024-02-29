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


    <!-- <div class="container">
      <h1 class="cartTitle">Cart</h1>
      <div class="itemsinCart"></div>
      <button class="checkOutbtn">Check Out</button>
    </div> -->
  </header>


</template>


<style scoped>
/* :root{
  --offwhite: #f1f8ff;
  --blue: #0073ff;
}
*/
.listing{
  display: flex;
    width: 75%;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 5px;
    flex-direction: row;
    border-style: solid;
    border-color: var(--blue);
    border-radius: 1rem;
    margin-top: 1.5rem;
}
/*
.container{
  background-color: var(--offwhite);
  color:var(--blue);
  width: 20%; height: 100%;
  float: right;
  position: absolute;
  top: 11rem;
  right: 2rem;
  overflow: scroll;
  overflow-y: auto;
  overflow-x: hidden;
  border-radius: 1rem;
  display: flex;
  align-items: center;
  flex-direction: column;
  border-style: solid;
  border-color: var(--blue);
}
*/
.title{
  font: 60px; text-align: center;
}
/*
.cartTitle, nav{
  text-align: center;
}
.checkOutbtn{
  background-color:var(--blue);
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
} */

</style>
