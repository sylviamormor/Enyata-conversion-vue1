<script setup>
import ButtonComponent from './components/ButtonComponent.vue';
import GreenComponent from './components/GreenComponent.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import NewcardsComponent from './components/NewcardsComponent.vue';
import PicturetextComponent from './components/PicturetextComponent.vue';
import TrendingComponentVue from './components/TrendingComponent.vue';
import GreenwhiteComponent from './components/GreenwhiteComponent.vue';
import SignupComponent from './components/SignupComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
import DealComponent from './components/DealComponent.vue';
</script>

<template>
  <div class="main">
    <HeaderComponent/>
  </div>
  <div class="section">
    <GreenComponent/>
  </div>
<div class="plainText">
  <p>Findtrend helps you to increase your
productivity and reduce your computer's
memory load, <span>an application that can 
fulfill your daily browsing needs. </span></p>
<p>Findtrend make +1000 Startup grow</p>

</div>
<div class="NComponent">
  <NewcardsComponent/>
  <p>All platform connect to Findtrend</p>
</div>
<div>
<TrendingComponentVue/>
</div>
 <PicturetextComponent/>
<div>
  <ButtonComponent/>
</div>
<DealComponent/>
<div>
  <SignupComponent/>
</div>
<div>
  <FooterComponent/>
</div>


  
</template>

<style scoped>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.main{
  background-color: black; 
  padding-bottom: 100px; 
  padding-right:30px ;      
}

.plainText{
  display: flex;
  flex-direction: column;
  gap: 160px;
  align-items: center;
  padding: 80px 18px;

}
.plainText p{
color: #000;
font-family: Effra;
font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: normal;
max-width: 335px;
align-items: center;
}

.plainText span{
color: #ADADAD;
font-family: Effra;
font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: normal;
max-width: 335px;
}

.NComponent{
  padding: 18px ;
 
}
.NComponent p{
color: #000;
text-align: center;
font-family: Effra;
font-size: 36px;
font-style: normal;
font-weight: 900;
line-height: normal;
padding-top: 160px;
/* max-width: 339px; */
}







@media (min-width: 750px) {
  .NComponent p{ 
  max-width: 1160px;
  }
  .plainText p{
    max-width: 1160px;
    padding:14px 10px ;

  }
  .gComponent{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding-bottom: 140px;
    background-color: #000;
  }

  




}
</style>


