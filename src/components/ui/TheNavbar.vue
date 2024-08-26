<script setup>
import { ref } from 'vue';
import { RouterLink } from 'vue-router';

const links = [
  {
    name: 'Home',
    path: '/',
  },
  {
    name: 'Sobre mim',
    path: '/about',
  },
  {
    name: 'Experiências',
    path: '/',
  },
  {
    name: 'Escolaridade',
    path: '/',
  },
  {
    name: 'Contato',
    path: '/',
  },
];

const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
}
</script>

<template>
  <div class="text-white text-2xl">
    <div @click="toggleMenu">
      {{ isMenuOpen ? '▲' : '▼' }}
    </div>

    <div class="lilita-one-regular" v-if="isMenuOpen">
      <nav class="flex flex-col">
        <template v-for="(link, index) in links" :key="index">
          <RouterLink :to="link.path" class="hover:underline" @click="toggleMenu">
            {{ link.name }}
          </RouterLink>
        </template>
      </nav>
    </div>
  </div>
</template>