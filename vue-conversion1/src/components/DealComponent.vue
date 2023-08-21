<script setup>
import DealcardComponent from './DealcardComponent.vue';
</script>

<template>
    <div class="dealcontainer">
        <h1 class="heading">Get your best deal</h1>
        <div class="togglepart">
            <h3 class="month">Monthly</h3>
            <label class="switch">
                <input type="checkbox">
                <span class="slider round"></span>
            </label>
            <div class="year">
                <h3 class="duration">Yearly</h3>
                <!-- <img src="" alt=" "> -->
            </div>
        </div>
        <div class="deals">
            <DealcardComponent class="deal1"/>
        </div>
    </div>
</template>

<style scoped>
    .deals{
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 20px;

    }
    .dealcontainer{
        background-color: #000;
        padding: 5% 5%;
        display: flex;
        flex-direction: column;
        gap: 20px;
        align-items: center;
    }
    .heading{
        color: #FFF;
        text-align: center;
        font-family: 'Ubuntu';
        font-size: 36px;
        font-style: normal;
        font-weight: 900;
        line-height: normal;
    }
    .togglepart{
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
    }
.switch {
  position: relative;
  display: inline-block;
  width: 80px;
  height: 34px;
}
.switch input {
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

/* Rounded sliders */
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
.duration{
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
.deal1, .deal3{
    background-color: #fff;
}
.deal2{
    background-color: #a8ff35;
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

.deals{
        display: flex;
        flex-direction: row;
        justify-content: center;
        gap: 10px;
          padding: 5% 5%;
}
.heading{
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