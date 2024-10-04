<script setup>
import iconMoon from '@/assets/img/icon-moon.svg'
import iconSun from '@/assets/img/icon-sun.svg'
</script>

<template class="hero">
    <div class="bg">
      <h1>Todo</h1>
      <img :src="iconMoon" alt="Moon Icon">
      <img :src="iconSun" alt="Sun Icon">
    </div>
  </template>
  
  <style scoped>
  .bg {
    background-image: url('@/assets/img/bg-desktop-dark.jpg');
    background-size: cover;
    background-position: center;
  }
  </style>