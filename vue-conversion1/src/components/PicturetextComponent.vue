<script setup >
import ButtonComponent from './ButtonComponent.vue';

</script>

<template>
<div class="mobilePix">
    <img src="../assets/tweetmobile1.png" alt="">
    <img src="../assets/tweetmobile2.png" alt="">
    <img src="../assets/tweetmobile3.png" alt="">
    
    <ButtonComponent class="newbtn"  buttontext="View more trend" />

</div>




</template>


<style scoped>
.mobilePix{
max-width: 800px;
padding: 32px 18px ;
display: flex;
flex-direction: column;
align-items: center;
justify-content: center;


}

.newbtn{ 
text-align: center;
padding: 12px 24px;
gap: 10px;
background: #000;
color: #FFF;
display: flex;
justify-content: center;
margin-top: 20px ;






}


@media (min-width: 900px) {
   
.mobilePix{
    display: flex;
    flex-direction: column;
    gap: 40px;
}

.btnblack{

justify-content: center;
align-items: center;
gap: 10px;
border-radius: 40px;
background: #000;
color: #FFF;
text-align: center;
font-family: Effra;
font-size: 14px;
font-style: normal;
font-weight: 700;
line-height: 140%;
}
}
</style>