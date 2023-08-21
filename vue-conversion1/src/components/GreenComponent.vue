<script setup>
import CardComponent from './CardComponent.vue';


</script>

<template>
    <div class="greenContent">

        <p class="greenText"> Open new tabs is sh*t</p>
        <div class="arrow1">
        <img src="../assets/mobilearrow1.png" alt="">
    </div>
        
        <div class="case1">
            <div cardCase>
                <CardComponent class="caseCard" Cardtext="Findtrend - Elon Musk" />
            </div>
            <div class="arrow2">
                <img src="../assets/mobilearrow2.png" alt="">
            </div>
            
        </div>
        <p class="greenPara">A solution for your browser tabs and don’t make your device get slower over time. Get ease and faster to discover a trend with just one tab.</p>

    </div>
</template>

<style scoped>
.greenContent {
    background-color: #A8FF35;
    padding: 18px 80px 18px 80px;
    display: flex;
    flex-direction: column;
    gap:20px ;
    align-items: center;
}

.greenText {
    color: #000;
    text-align: center;
    font-family: Effra;
    font-size: 36px;
    font-style: normal;
    font-weight: 700;
    line-height: 112%;
}

.case1 {
    width: 339px;
    height: 118px;
    padding: 20px 20px;
    border-radius: 14px;
    background: #F5F5F5;


}
.greenPara{
   max-width: 286px; 
   color: #000;
text-align: center;
font-family: Effra;
font-size: 14px;
font-style: normal;
font-weight: 400;
line-height: 150%
}


.arrow1  {
   position: absolute;
   right: 0%;  
}

.arrow2 img{
    position: absolute;
    left: 0%;
}







@media (min-width: 750px) {
.arrow1 {
   position: absolute;
  
}

.arrow2{
    position: absolute;
    left: 0%;
}
.case1{
    max-width: 502px;
}
}
</style>