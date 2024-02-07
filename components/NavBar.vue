<template>
    <div class="nav-bar">
        <div class="logo">
            <img src="../static/logo.png" alt="logo">
        </div>
        <div class="search-bar">
            <i class="ri-search-line"></i>
            <input type="text" placeholder="Search Movies, TV, Actore, More ...">
        </div>
        <div class="nav-links">
            <div class="sign-links">
                <NuxtLink class="custom-link" to="/" >What's the Tomatometer?</NuxtLink>
                <NuxtLink class="custom-link" to="/" >Critics</NuxtLink>
                <NuxtLink class="custom-link" to="/" >LOGIN/SIGNUP</NuxtLink>
            </div>
            <div class="show-links">
                <NuxtLink class ="link" to="/">Movies</NuxtLink>
                <NuxtLink class ="link" to="/">TV Shows</NuxtLink>
                <NuxtLink class ="link" to="/">Shop</NuxtLink>
                <NuxtLink class ="link" to="/">News</NuxtLink>
                <NuxtLink class ="link" to="/">Showtime</NuxtLink>
            </div>
        </div>
    </div>
  
</template>

<script>
export default {
  name:'NavBar'
}
</script>

<style  scoped>
@import 'remixicon/fonts/remixicon.css';
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
.search-bar {
  position: relative;
  width: 700px;
  margin: 10px 60px;
}

.search-bar i {
  position: absolute;
  top: 50%;
  left: 20px;
  transform: translateY(-50%);
  color: white;
  font-size: 1.5rem;
}

.search-bar input {
  width: 100%;
  padding: 14px 60px;
  background-color: rgb(150, 30, 6);
  color: white;
  font-size: 1.3rem;
  font-weight: 600;
  border-radius: 50px;
  border: 2px solid white;
}

::placeholder {
  color: white;
  font-size: 1.3rem;
}
.nav-links{
   display: flex;
   align-items: center;
   flex-direction: column;
   gap:50px;
   list-style: none;
   text-decoration: none;
   margin: 10px 80px;
   color: white;
}
.sign-links .custom-link{
     text-decoration: none;
     color: white;
     font-size: 1.3rem;
     font-weight: 600;
     padding: 0px 50px;
}
.show-links .link{
     text-decoration: none;
     color: white;
     font-size: 1.7rem;
     font-weight: 600;
     padding: 10px 20px;
     text-transform: uppercase;
     margin-bottom: 20px;
}
</style>