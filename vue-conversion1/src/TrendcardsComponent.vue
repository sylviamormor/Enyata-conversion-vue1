<script setup>
 defineProps(["trend"])
</script>

<template>
  <div class="trendIcons">
   <img :src="trend">
    
  </div>
</template>

<style scoped>
.trendIcons{
width: 64px;
height: 64px;
border-radius: 8px;
display: flex;
gap:20px ;
text-align: center;
background-color: white;
}
</style>
