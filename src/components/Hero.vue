<script setup>
import iconMoon from '@/assets/img/icon-moon.svg'
import iconSun from '@/assets/img/icon-sun.svg'

import { ref } from 'vue';

const isDarkMode = ref(document.documentElement.getAttribute('data-theme') === 'dark');

function toggleTheme() {
  isDarkMode.value = !isDarkMode.value;
  document.documentElement.setAttribute('data-theme', isDarkMode.value ? 'dark' : 'light');
}
</script>

<template class="hero">
    <div class="bg">
      <h1>Todo</h1>
      <a @click.prevent="toggleTheme">
        <img :src="isDarkMode ? iconMoon : iconSun" alt="Toggle Theme" />
      </a>
      <!-- <img :src="iconMoon" alt="Moon Icon">
      <img :src="iconSun" alt="Sun Icon"> -->
    </div>
  </template>
  
  <style scoped>
  .bg {
    background-image: url('@/assets/img/bg-desktop-light.jpg');
    background-size: cover;
    background-position: center;
  }
  </style>