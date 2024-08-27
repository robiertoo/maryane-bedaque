<script setup>
import { faInstagram, faWhatsapp } from '@fortawesome/free-brands-svg-icons';
import { faChevronCircleDown, faChevronCircleUp, faEnvelope } from '@fortawesome/free-solid-svg-icons';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { ref } from 'vue';

const isIconPressed = ref(false);

const handleClick = () => {
  isIconPressed.value = !isIconPressed.value;
};
</script>

<template>
  <div class="fixed bottom-5 right-5">
    <font-awesome-icon
      @click="handleClick"
      :icon="isIconPressed ? faChevronCircleDown : faChevronCircleUp"
      class="text-3xl"
    />

    <div v-show="isIconPressed" class="fixed bottom-16 right-5">
      <div class="flex flex-col space-y-3 justify-center items-center">
          <a
            href="https://wa.me/5511999999999"
            class="font-bold underline text-3xl"
            target="_blank"
          >
            <font-awesome-icon :icon="faWhatsapp" />
          </a>

          <a href="mailto:Jpj4h@example.com" class="font-bold underline text-3xl" target="_blank">
            <font-awesome-icon :icon="faEnvelope" />
          </a>

          <a
            href="https://www.instagram.com/maryanebedaque.di/"
            class="font-bold underline text-3xl"
            target="_blank"
          >
            <font-awesome-icon :icon="faInstagram" />
          </a>
        </div>
    </div>
  </div>
</template>