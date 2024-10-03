<script setup>
import icon from '@/assets/img/icon-moon.svg'
</script>

<template class="hero">
    <div class="bg">
      <h1>Todo</h1>
      <img :src="icon" alt="Moon Icon">
    </div>
  </template>
  
  <style scoped>
  .bg {
    background-image: url('@/assets/img/bg-desktop-dark.jpg');
    background-size: cover;
    background-position: center;
  }
  </style>