<script setup>
import iconSun from '@/assets/img/icon-sun.svg'
import iconMoon from '@/assets/img/icon-moon.svg'
</script>

<template class="hero">
    <div class="bg">
      <h1>Todo</h1>
      <img :src="iconSun" alt="Sun Icon">
      <img :src="iconMoon" alt="Moon Icon">
    </div>
  </template>
  
  <style scoped>
  .bg {
    background-image: url('@/assets/img/bg-desktop-light.jpg');
    background-size: cover;
    background-position: center;
  }
  </style>