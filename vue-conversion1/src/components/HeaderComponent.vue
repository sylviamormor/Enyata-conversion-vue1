<script setup>
import ButtonComponent from './ButtonComponent.vue';
import CardComponent from './CardComponent.vue';
import twitter from '../assets/twitter.png'
import pintrest from '../assets/pintrest.png'
import facebook from '../assets/facebook.png'
import pink from '../assets/pink.png'
</script>

<template>
  <div class="header">
    <nav class="navBar">
      <div class="logo">
        <img src="../assets/Vectorfindlogo.png" alt="">
        <p>Findtrend</p>
      </div>
      <div class="navList">
        <a href="">About</a>
        <a href="">How it works</a>
        <a href="">Pricing</a>
        <a href="">Solution</a>
        <a href="">Features</a>
      </div>
      <div class="navBtns">
        <a href="" class="login">Login</a>
        <ButtonComponent buttontext="Register" />
      </div>
      <div class="menu">
        <img src="../assets/iconmenu.png" alt="">
      </div>
    </nav>
  </div>
  <div class="headerText">
    <h1>Minimize your tabs. <br> Find the trends! </h1>
    <p>Don’t let your computer memories consumes all of those browser tabs.
      Findtrend let you gathers all of your favorite website into one place.</p>
    <div>
      <ButtonComponent class="greenBtn" buttontext="Get Started 🔥" />
    </div>
    <div class="allCards">
      <CardComponent class="card1" :images="twitter" Cardtext="Cryptopunk - Search" />
      <CardComponent class="card2" :images="pintrest" Cardtext="Popular Design - Search" />
      <CardComponent class="card3" :images="facebook" Cardtext="Product Design - Search" />
      <CardComponent class="card4" :images="pink" Cardtext="Elon Musk - Search" />
    </div>
  </div>
</template>




<style scoped>
.navBar {
  display: flex;
  justify-content: space-between;
  background-color: black;
  align-items: center;
  padding: 30px 18px;
}

.navBar p {
  display: none;
}

.logo {
  display: flex;
  width: 100px;
  height: 40px;
  align-items: center;

}


.navList {
  display: none
}

.navBtns {
  display: none;
}

.login {
  display: none;
}

.greenBtn {
  color: #000;
  text-align: center;
  font-family: Effra;
  font-size: 14px;
  font-style: normal;
  font-weight: 700;
  line-height: 140%;
  border-radius: 40px;
  background: #A8FF35;
}


.headerText {
  display: flex;
  flex-direction: column;
  gap: 32px;
  background-color: #000;
  align-items: center;
}

.headerText h1 {
  color: #FFF;
  text-align: center;
  font-family: Effra;
  font-size: 36px;
  font-style: normal;
  font-weight: 900;
  line-height: 112%;
}

.headerText p {
  color: #8B8B8B;
  text-align: center;
  font-family: Effra;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: 150%;
  max-width: 286px;
  margin: auto;
}


.card1{
  transform: rotate(-4deg);
}

.card2 {
  transform: rotate(2deg);
}

.card3 {
  transform: rotate(-2deg);
}

.card4 {
  transform: rotate(4deg);
}










@media (min-width: 900px) {

  .navList {
    display: flex;
    gap: 20px;
  }

  .navList a {
    text-decoration: none;
    list-style: none;
    color: white;
    align-items: center;
  }

  .navBar p {
    display: block;
    color: white;
  }

  .login {
    display: block;
    text-decoration: none;
    color: white;
  }

  .navBtns {
    display: flex;
    gap: 10px;
    align-items: center;
  }

  .menu {
    display: none;
  }


  .allCards {
    display: flex;
    position: relative;
    flex-direction: row;
    gap: 20px;
   
  }

  .card2 {
   
    position: relative;
  }

  .card1 {
    position:absolute ;
    top: 80%;
    right: 80%;
    
  }

  .card3 {
    position: relative;
  }

  .card4{
    position: absolute;
    right: 0%;
    top: 40%;
    z-index: 2;
  }

  












}
</style>