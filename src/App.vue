<script setup>
import LaundryCalculator from './components/LaundryCalculator.vue';
import NavBar from './components/NavBar.vue';
</script>

<template>
  <NavBar/>
  <div class="app">
    <h1 class="title">Selamat Datang di Aplikasi Laundry Calculator</h1>
    <LaundryCalculator msg="Vite + Vue" />
  </div>
</template>

<style scoped>
.title {
  font-size: 2em;
  margin-bottom: 30px;
  color: #000000;
}

.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 1em #ff6480aa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 1em #42b883aa);
}
</style>
