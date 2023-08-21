<script setup>
import ButtonComponent from './ButtonComponent.vue';


</script>

<template>
    <div class="signup">
        <h1 class="signupText">Join us on email for</h1>
        <div class="joinNow">more trending topics</div>
        <ButtonComponent class="btn" buttontext="Join Now"/>
    </div>
</template>

<style scoped>
.signup{
    padding: 10%;
    background: #A8FF35;
    display: flex;
    justify-content: center;
    flex-direction: column;
    
}
    .signupText{
        color: #000;
        text-align: center;
        font-size: 36px;
        font-style: normal;
        font-weight: 900;
        line-height: 40px;
    }
    .joinNow{
        color: #87D322;
        text-align: center;
        font-size: 36px;
        font-style: normal;
        font-weight: 900;
        line-height: 40px;
        margin-bottom: 20px;
    }
    .btn{
        margin: 0 auto;
        background-color: #000;
        color: #fff;
    }
    @media (min-width: 900px){
        .signupText{
        color: #000;
        text-align: center;
        font-size: 72px;
        font-style: normal;
        font-weight: 900;
        line-height: 80.64px;
    }
    .joinNow{
        color: #87D322;
        text-align: center;
        font-size: 72px;
        font-style: normal;
        font-weight: 900;
        line-height: 40px;
        margin-bottom: 20px;
    }
    }
</style>