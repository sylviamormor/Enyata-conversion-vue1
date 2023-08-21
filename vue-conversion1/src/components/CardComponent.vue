<script setup>
defineProps(["images", "Cardtext"])
</script>

<template>
    <div class="cards">
        <img :src= "images">
        <p>{{ Cardtext }}</p>
        <div class="close-icon">
            <img src="../assets/close-icon.png"/>

        </div>

    </div>

</template>

<style scoped>
.cards{
width: 293.038px;
height: 70.42px;
background: #181818;
display: flex;
gap: 8px ;
align-items: center;
padding: 20px 30px;
display: flex;
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