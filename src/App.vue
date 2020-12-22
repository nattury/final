<template>
  <div class="comun">
    <header class="encabezado">
      <a href="/"><img src="./assets/logo.png" class="logo" alt="logo"></a>
      
      <ul class="menu">
        <li><a class="links" href="/about">About</a></li>
        <li><a class="links" href="/rooms">Rooms</a></li>
        <li><a class="links" href="/client/mybooking/">My&nbsp;&nbsp;Booking</a></li>
        <li><a class="links" href="">Contact</a></li>
      </ul>
    </header>

<!-- <main class="principal">
       <div class="contenedor">
            <ul class="redes">
                <li class="sociales"><a href="https://mail.google.com/" target="_blank" class="link_redes"></a><i class="fa fa-at gmail icon"></i></li>
                <li class="sociales"><a href="https://twitter.com/" target="_blank" class="link_redes"></a><i class="fa fa-twitter twitter icon"></i></li>
                <li class="sociales"><a href="https://www.facebook.com/" target="_blank" class="link_redes"></a><i class="fa fa-facebook facebook icon"></i></li>
                
            </ul>
            </div>
        <p class="info">¡Hello there! <br>
            It is nice to see you. <br><br>
            It is a pleasure for us that you come to our facilities. Here will be the place where you will be <br>
            like home with the most comfortable and relaxing rooms and service.</p>
    </main> -->

    <div class="main-component">
      <router-view></router-view>
    </div>
    
  </div>
</template>



<script>

import Router from 'vue-router'

export default {
  name: "App",
};
</script>

<style>

.comun {
  margin: 0;
  padding: 0;
  /* box-sizing: border-box; */
  color: white;
  font-family: "Yanone Kaffeesatz", sans-serif;
  font-size: 27px;
}

body {
  background-image: url(./assets/mountain.jpg);
  width: 100%;
  background-attachment: fixed;
  background-size: cover;
}

.encabezado {
  display: flex;
  justify-content: space-between;
  /* padding: 30px 40px; */
  padding-right: 50px;
}


.menu {
  display: flex;
  justify-content: space-around;
  align-items: center;
  list-style: none;
  padding-right: 40px;
}

.menu a:link{
  color: white;
}
.menu a:visited{
  color: white;
}

.links {
  text-decoration: none;
  padding: 40px ;
  margin: 10px;
}

.logo{
  width: 29%;
}

/* @media screen and (min-width: 800px){
  body{
    background: #ff8000;
  }
} */

@media (max-width: 800px){
  .comun{
    font-size: 12px;
  }
}
    
</style>
