<template>
  <div>
    <main class="principal">
       <div class="contenedor">
            <ul class="redes">
                <li class="sociales"><a href="https://mail.google.com/" target="_blank" class="link_redes"></a><i class="fa fa-at gmail icon"></i></li>
                <li class="sociales"><a href="https://twitter.com/" target="_blank" class="link_redes"></a><i class="fa fa-twitter twitter icon"></i></li>
                <li class="sociales"><a href="https://www.facebook.com/" target="_blank" class="link_redes"></a><i class="fa fa-facebook facebook icon"></i></li>
                
            </ul>
            </div>
        <p class="info">¡Hello there! <br>
            It is nice to see you. <br><br>
            It is a pleasure for us that you come to our facilities. Here will be the place where you will be
            like home with the most comfortable and relaxing rooms and service.</p>
    </main>
    <footer class="foot">
      <p>Book with us <br />and enjoy special benefits</p>
      <ul class="menubajo">
        <li><a class="links" href="/locate">Locate</a></li>
        <li>
          <a class="links" href="https://www.apple.com/co/app-store/" target="_blank"
            >Download&nbsp;&nbsp;App</a
          >
        </li>
        <li><a class="links" href="">Guest</a></li>
      </ul>
    </footer>
  </div>
</template>
<script>
export default {
  name: "Principal",
};
</script>
<style>

.principal{
    display: grid;
    grid-template-columns: 1fr 4fr;
}

.contenedor {
    height: 300px;
    width: 300px;
    margin: 120px 0;
}

.redes {
    margin-left: -1%;
    width: 70%;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    cursor: pointer;
    position: fixed;
}

.sociales {
    position: relative;
    transform: translateX(-50px);
    background: rgba(50, 50, 85, 0.418);
    list-style: none;
    padding: 10px 0;
    transition: 0.5s;
    width: 100px;
    border-radius: 0 200px 200px 0;
    cursor: pointer;

}

.sociales:hover:nth-child(1){
    background:  #42858a;
}
.sociales:hover:nth-child(2){
    background: #42858a;
}
.sociales:hover:nth-child(3){
    background:  #42858a;
}
.sociales:hover{
    transform: translateX(0);
}
.link_redes{
    font-weight: bold;
    color: #fff;
    text-decoration: none;
    padding-left: 10px;
}

 
.gmail{
    position: relative;
    left: 30px;
}
.twitter{
    position: relative;
    left: 30px;
}
.facebook{
    position: relative;
    left: 30px;
    }

.info {
  padding-top: 40%;
  width: 80%;
}

.foot {
  background: rgba(118, 164, 175, 0.459);
  padding: 0 50px;
  width: 70%;
  height: 18%;
  position: absolute;
  bottom: 20px;
  margin-left: 18%;
  margin-right: 20%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.foot ul {
  list-style: none;
  display: flex;
  justify-content: space-around;
}

.foot a:link {
  color: white;
}
.foot a:visited {
  color: white;
}

.menubajo{
  width: 65%;
}

@media(max-width: 800px){
  .foot {
    width: 90%;
  }

  .contenedor{
    width: 60%;
  }
  }
  
</style>
