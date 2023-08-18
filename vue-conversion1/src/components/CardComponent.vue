<script setup>
defineProps(["Cardtest"])
</script>

<template>
    <div class="cards">
        <img src="../assets/image 96twitter.png" alt="">
        <p>{{ Cardtest }}</p>

    </div>

</template>

<style scoped>
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

.cards p{
color: #FFF;
text-align: center;
font-family: Roboto;
font-size: 20.445px;
font-style: normal;
font-weight: 400;
line-height: normal;
}



</style>