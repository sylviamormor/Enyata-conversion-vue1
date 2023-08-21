<script setup>

import GreencardComponent from './GreencardComponent.vue';
</script>

<template>
    <div class="container">
        <h1 class="header">Get your best deal</h1>
        <div class="body">
            <h3 class="month">Monthly</h3>
            <label class="choose">
                <input type="checkbox">
                <span class="slider round"></span>
            </label>
            <div class="year">
                <h3 class="period">Yearly</h3>
                <img src="../assets/toogler.png" alt=" ">
            </div>
        </div>
        <div class="deals">
            <GreencardComponent class="deal1"/>
        </div>
    </div>
</template>

<style scoped>
    .deals{
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 20px;

    }
    .container{
        background-color: #000;
        padding: 10%;
        display: flex;
        flex-direction: column;
        gap: 30px;
    }
    .header{
        color: #FFF;
        text-align: center;
        font-family: 'Ubuntu';
        font-size: 36px;
        font-style: normal;
        font-weight: 900;
        line-height: normal;
    }
    .body{
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
    }
.choose {
  position: relative;
  display: inline-block;
  width: 80px;
  height: 34px;
}
.choose input {
  opacity: 0;
  width: 0;
  height: 0;
}
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: .4s;
  transition: .4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 26px;
  width: 26px;
  left: 4px;
  bottom: 4px;
  background-color: rgba(168, 255, 53, 1);
  -webkit-transition: .4s;
  transition: .4s;
}

input:checked + .slider {
  background-color: #FFF;
}

input:focus + .slider {
  box-shadow: 0 0 1px #FFF;
}

input:checked + .slider:before {
  -webkit-transform: translateX(45px);
  -ms-transform: translateX(45px);
  transform: translateX(45px);
}


.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}
.month{
    color: #FFF;
    font-family: 'Ubuntu';
    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
}
.period{
    color: #F5F5F5;
    font-family: 'Ubuntu';
    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
}
.year{
    position: relative;
}
.year img{
    position: absolute;
}


@media (min-width: 900px){
    .year{
    position: static;
    display: flex;
    align-items: center;
    gap: 10px;
}
.year img{
    position: static;
}
.header{
    color: #FFF;
    text-align: center;
    font-family: 'Ubuntu';
    font-size: 64px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

}
</style>