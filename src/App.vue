<script setup>
import { RouterView } from 'vue-router';
import TheNavbar from './components/ui/TheNavbar.vue';
</script>

<template>
  <div class="p-2 space-y-2">
    <header>
      <the-navbar />
    </header>

    <div class="py-2 md:px-32">
      <router-view />
    </div>
  </div>
</template>
