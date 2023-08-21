<script setup>
import ButtonComponent from './ButtonComponent.vue';
import GreentextComponent from './GreentextComponent.vue';
import GreenwhiteComponent from './GreenwhiteComponent.vue';
    
</script>

<template>
  <div>
    <GreenwhiteComponent/>
  
       
    <div class="dcontainer deal1">
        <h1 class="info">Personal</h1>
        <p class="page">Special first packet for all</p>
        <hr>
        <h1 class="dollars">$8 <small>/month</small></h1>
        <GreentextComponent deallist="Up to 5 page each group"/>
        <GreentextComponent deallist="Up to 10 page"/>
        <GreentextComponent deallist="5 Days group page saved"/>
        <GreentextComponent deallist="Up to 1 each group"/>
        <GreentextComponent deallist="Up to 2 page each group"/>
        <ButtonComponent  buttontext="Start Free Trial" class="blackbutton"/>
        
    </div>
    <div class="dcontainer deal2">
        <h1 class="info">Regular</h1>
        <p class="page">Recommended for personal pro</p>
        <hr>
        <h1 class="dollars">$20 <small>/month</small></h1>
        <GreentextComponent deallist="Up to 5 page each group"/>
        <GreentextComponent deallist="Up to 10 page"/>
        <GreentextComponent deallist="5 Days group page saved"/>
        <GreentextComponent deallist="5 Days group page saved"/>
        <GreentextComponent deallist="5 Days group page saved"/>
        <ButtonComponent buttontext="Start Free Trial" class="greenbtn"/>
    </div>
    <div class="dcontainer deal3">
        <h1 class="info">Premium</h1>
        <p class="page">Packet for Startup & Company</p>
        <hr>
        <h1 class="dollars">$48 <small>/month</small></h1>
        <GreentextComponent deallist="Up to 5 page each group"/>
        <GreentextComponent deallist="Up to 10 page"/>
        <GreentextComponent deallist="5 Days group page saved"/>
        <GreentextComponent deallist="5 Days group page saved"/>
        <GreentextComponent deallist="5 Days group page saved"/>
        <ButtonComponent  buttontext="Start Free Trial" class="blackbutton"/>
    </div>
</div>
</template>

<style scoped>
.dcontainer{
    position: relative;
    padding: 15px;
    border-radius: 16px;
    display: flex;
    flex-direction: column;
    gap: 10px;
    justify-content: space-between;
}   
.deal1, .deal3{
    background-color: #fff;
}
.deal2{
    background-color: #a8ff35;
}
.blackbutton{
    background-color: #a8ff35;
    margin:0 auto;
}
.greenbtn{
    background-color: #000;
    margin:0 auto;
    color: #fff;
}
small{
    color: #000;
font-family: Effra;
font-size: 18px;
font-style: normal;
font-weight: 400;
line-height: 18px;
}
.dollars{
    color: #000;
    font-size: 64px;
    font-style: normal;
    font-weight: 400;
    line-height: 100%; 
}
@media (min-width: 900px){
    
}

</style>