<script setup>
    defineProps(['deallist'])
</script>

<template>
    
    <div class="pages">
        <img src="../assets/checked.png" alt="">
        <p class="lists">{{ deallist }}</p>
    </div>
</template>

<style scoped>
    .pages{
        display: flex;
        gap: 10px;
    }
    .lists{
        color: #000;
font-size: 16px;
font-style: normal;
font-weight: 400;
line-height: 18px;
    }
</style>