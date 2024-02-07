<template>
  <div class="container">
     <div class="nav-bar">
          <div class="logo">
              <img src="../static/logo.png" alt="logo">
          </div>
          <div class="search-bar">
            <i class="ri-search-line"></i>
            <input type="text" placeholder="Search Movies, TV, Actore, More ...">
          </div>
          <div class="nav-links">
            <ul>
              <NuxtLink to="/">Movies</NuxtLink>
              <NuxtLink to="/">TV Shows</NuxtLink>
              <NuxtLink to="/">Shop</NuxtLink>
              <NuxtLink to="/">News</NuxtLink>
              <NuxtLink to="/">Showtime</NuxtLink>
            </ul>
          </div>

     </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
<style>
.logo{
   margin: 10px 20px;
   padding: 20px;
}
.nav-bar {
   width: 100%;
   height: 150px;
   display: flex;
   align-items: center;
   justify-content: space-between;
   background-color: rgb(250,50,10);
}
.search-bar input{
   width:600px;
   margin: 10px 20px;
   padding: 14px 40px;
   background-color: rgb(150,30,6);
   color: white;
   font-size: 1.3rem;
   font-weight: 600;
   border-radius: 50px;
   border: 2px solid white;
}
.nav-links{
   display: flex;
   align-items: center;
   list-style: none;
   text-decoration: none;
   margin: 10px 80px;
   color: white;
   text-transform: capitalize;
   font-size: 2rem;
}
</style>