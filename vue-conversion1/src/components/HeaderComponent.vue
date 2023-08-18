<script setup>
import ButtonComponent from './ButtonComponent.vue';
import CardComponent from './CardComponent.vue';
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
      <ButtonComponent buttontext="Register"/>
    </div>
    <div class="menu">
      <img src="../assets/iconmenu.png" alt="">
    </div>
  </nav>
</div>
<div class="headerText">
  <h1>Minimize your tabs. <br> Find the trends!   </h1>
  <p>Don’t let your computer memories consumes all of those browser tabs. 
Findtrend  let you gathers all of your favorite website into one place.</p>
<div>
<ButtonComponent class="greenBtn" buttontext="Get Started 🔥"/>
</div>
<div>
  <CardComponent class="card1" Cardtest="Cryptopunk - Search"/>
  <CardComponent class="card2" Cardtest="Popular Design - Search"/>
  <CardComponent class="card3" Cardtest="Product Design - Search"/>
  <CardComponent class="card4" Cardtest="Elon Musk - Search"/>
    </div>
</div>

</template>




<style scoped>


.navBar{
  display: flex;
  justify-content: space-between;
  background-color: black;
  align-items: center;
  padding: 30px 18px;
}

.navBar p{
  display: none;
}
.logo{
  display: flex;
  width: 100px;
  height: 40px;
  align-items: center;

}


.navList{
  display: none
}

.navBtns{
  display: none; 
}

.login{
  display: none;
}

.greenBtn{
color: #000;
text-align: center;
font-family: Effra;
font-size: 14px;
font-style: normal;
font-weight: 700;
line-height: 140%; /* 19.6px */
border-radius: 40px;
background: #A8FF35;
}

.headerText{
  display: flex;
  flex-direction: column;
  gap: 32px;
  background-color: #000;
  align-items: center;
}

.headerText h1{
  color: #FFF;
text-align: center;
font-family: Effra;
font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: 112%; /* 40.32px */
}

.headerText p{
  color: #8B8B8B;
text-align: center;
font-family: Effra;
font-size: 14px;
font-style: normal;
font-weight: 400;
line-height: 150%; /* 21px */
max-width: 286px; 
margin: auto;
}

.cards{
width: 293.038px;
height: 70.42px;
transform: rotate(-4deg);
background: #181818;
display: flex;
gap: 8px ;
align-items: center;
padding: 20px 30px;
}

.card1 p{
  max-width: 70px;

}
.cards p{
color: #FFF;
text-align: center;
font-family: Roboto;
font-size: 20.445px;
font-style: normal;
font-weight: 400;
line-height: normal;
}









@media (min-width: 750px){

.navList{
  display: flex;
  gap: 20px;
}

.navList a{
  text-decoration: none;
  list-style: none;
  color: white;
  align-items: center;
}

.navBar p{
  display: block;
  color: white;
}
.login{
  display: block;
  text-decoration: none;
  color: white;
}

.navBtns{
  display: flex;
  gap: 10px;
  align-items: center;
}

.menu{
  display: none;
}

} 

</style>