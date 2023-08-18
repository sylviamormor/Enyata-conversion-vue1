<script setup>
defineProps(["buttontext"])
</script>

<template>
<button>{{ buttontext }}</button>
</template>

<style scoped>
 button{
    border-radius: 40px;
    background: #FFF;
    border: none;
    color: #000;
text-align: center;
font-family: Effra;
font-size: 18px;
font-style: normal;
font-weight: 400;
line-height: 18px; 
padding: 12px 32px ;
    

 }

</style>
