<script setup>
    defineProps(['deallist'])
</script>

<template>
    
    <div class="page">
        <img src="../assets/checked.png" alt="">
        <p class="listp">{{ deallist }}</p>
    </div>
</template>

<style scoped>
    .page{
        display: flex;
        gap: 10px;
    }
    .listp{
        color: #000;
font-size: 16px;
font-style: normal;
font-weight: 400;
line-height: 18px;
    }
</style>