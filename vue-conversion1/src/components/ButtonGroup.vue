<script setup>
 const emit = defineEmits(["the-yes", "the-no"]);
</script>

<template>
  <div>
   
    <button @click="emit('the-yes')">Yes</button>
    <button @click="emit('the-no')">No</button>
  </div>
</template>

<style scoped>

</style>

<!-- <ButtonGroup @the-yes="handleyes" @the-no="handleno"/> -->