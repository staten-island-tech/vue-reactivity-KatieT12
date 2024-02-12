<script setup>
// import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <h1 class="title">Cars</h1>
    
    <!-- <div class="cart">
        <h1>Cart</h1>
      </div> -->
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" /> -->
    
    <div class="wrapper">

      <nav>
        <RouterLink to="/about">Products</RouterLink>
        <RouterLink to="/about">Cart</RouterLink>
        <Router-view />
      </nav>

      
    </div>
  </header>

</template>

<style scoped>

.title{
  margin-left: auto; margin-right: auto;
}
.cart{
  background-color: aquamarine;
  height: 150px;
  
  /* display: flex;
  align-items: right; */
  text-align: left;
  /* float: right; */

}
</style>