<script setup>
import { computed, ref } from 'vue';
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
const isMobile = computed(() => window.innerWidth < 768);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
}
</script>

<template>
  <div class="text-white text-2xl">
    <div @click="toggleMenu" v-if="isMobile" class="cursor-pointer">
      {{ isMenuOpen ? '▲' : '▼' }}
    </div>

    <div class="lilita-one-regular" v-show="isMenuOpen || !isMobile">
      <nav class="flex flex-col md:flex-row md:justify-around md:px-24 lg:px-52">
        <template v-for="(link, index) in links" :key="index">
          <RouterLink :to="link.path" class="hover:underline" @click="toggleMenu">
            {{ link.name }}
          </RouterLink>
        </template>
      </nav>
    </div>
  </div>
</template>