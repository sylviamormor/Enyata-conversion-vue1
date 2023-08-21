<script setup>
 defineProps(["social"])
</script>

<template>
  <div class="socialIcons">
   <img :src="social">
    
  </div>
</template>

<style scoped>
.socialIcons{
display: flex;
align-items: center;
justify-content: center;
border-radius: 8px;
background: #F5F5F5;
padding: 14px;

}
</style>