<script setup>

import GreencardComponent from './GreencardComponent.vue';
</script>

<template>
    <div class="mainContainer">
        <h1 class="header">Get your best deal</h1>
        <div class="body">
            <h3 class="month">Monthly</h3>
            <img src="../assets/slider.png" alt=" ">
            <div class="year">
                <h3 class="period">Yearly</h3>
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
    .mainContainer{
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
    /* position: static; */
    display: flex;
    align-items: center;
    gap: 10px;
}
/* .year img{
    position: static;
} */
.header{
    color: black;
    text-align: center;
    font-family: 'Ubuntu';
    font-size: 64px;
    font-style: normal;
    font-weight: 900;
    line-height: normal;
}

}
</style>