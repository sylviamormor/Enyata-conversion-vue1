<script setup>
import ButtonComponent from './ButtonComponent.vue';
import TextDealComponent from './TextDealComponent.vue';
    
</script>

<template>
    <div class="dcontainer deal1">
        <h1 class="info">Personal</h1>
        <p class="infop">Special first packet for all</p>
        <hr>
        <h1 class="currency">$8 <small>/month</small></h1>
        <TextDealComponent deallist="Up to 5 page each group"/>
        <TextDealComponent deallist="Up to 10 page"/>
        <TextDealComponent deallist="5 Days group page saved"/>
        <TextDealComponent deallist="Up to 1 each group"/>
        <TextDealComponent deallist="Up to 2 page each group"/>
        <ButtonComponent  buttontext="Start Free Trial" class="btnblack"/>
        
    </div>
    <div class="dcontainer deal2">
        <h1 class="info">Regular</h1>
        <p class="infop">Recommended for personal pro</p>
        <hr>
        <h1 class="currency">$20 <small>/month</small></h1>
        <TextDealComponent deallist="Up to 5 page each group"/>
        <TextDealComponent deallist="Up to 10 page"/>
        <TextDealComponent deallist="5 Days group page saved"/>
        <TextDealComponent deallist="5 Days group page saved"/>
        <TextDealComponent deallist="5 Days group page saved"/>
        <ButtonComponent  buttontext="Start Free Trial" class="btngreen"/>
    </div>
    <div class="dcontainer deal3">
        <h1 class="info">Premium</h1>
        <p class="infop">Packet for Startup & Company</p>
        <hr>
        <h1 class="currency">$48 <small>/month</small></h1>
        <TextDealComponent deallist="Up to 5 page each group"/>
        <TextDealComponent deallist="Up to 10 page"/>
        <TextDealComponent deallist="5 Days group page saved"/>
        <TextDealComponent deallist="5 Days group page saved"/>
        <TextDealComponent deallist="5 Days group page saved"/>
        <ButtonComponent  buttontext="Start Free Trial" class="btnblack"/>
    </div>
</template>

<style scoped>
.dcontainer{
    padding: 15px;
    border-radius: 16px;
    display: flex;
    flex-direction: column;
    gap: 10px;
    justify-content: space-between;
    width: 339px;
}   
.deal1, .deal3{
    background-color: #fff;
}
.deal2{
    background-color: #a8ff35;
}
.btnblack{
    background-color: #a8ff35;
    margin:0 auto;
}
.btngreen{
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
.currency{
    color: #000;
    font-size: 64px;
    font-style: normal;
    font-weight: 400;
    line-height: 100%; 
}
@media (min-width: 785px){
    
}

</style>