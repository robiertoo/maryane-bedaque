<script setup>
import { computed } from 'vue';
import AboutView from './views/AboutView.vue';
import ContactView from './views/ContactView.vue';
import EducationView from './views/EducationView.vue';
import HomeView from './views/HomeView.vue';
import WorkExperienceView from './views/WorkExperienceView.vue';
import FloatingButton from './components/ui/FloatingButton.vue';

const isMobile = computed(() => window.innerWidth < 768);
</script>

<template>
  <div class="">
    <home-view />
    <about-view />
    <work-experience-view />
    <education-view />
    <contact-view v-if="!isMobile"/>

    <floating-button />
  </div>
</template>
