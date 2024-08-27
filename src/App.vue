<script setup>
import AboutView from './views/AboutView.vue';
import ContactView from './views/ContactView.vue';
import EducationView from './views/EducationView.vue';
import HomeView from './views/HomeView.vue';
import WorkExperienceView from './views/WorkExperienceView.vue';
</script>

<template>
  <div class="p-2 space-y-2">
    <div class="py-2 md:px-32">
      <home-view class="min-h-screen" />
      <about-view class="min-h-screen" />
      <work-experience-view class="min-h-screen" />
      <education-view class="min-h-screen" />
      <contact-view class="min-h-screen" />
    </div>
  </div>
</template>
