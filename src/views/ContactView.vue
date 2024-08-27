<script setup>
import Page from '@/components/ui/Page.vue';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { faWhatsapp, faInstagram } from '@fortawesome/free-brands-svg-icons';
import { faEnvelope } from '@fortawesome/free-solid-svg-icons';
</script>

<template>
  <page id="contact" class="flex flex-col md:flex-row md:space-x-4 space-y-2">
    <div class="w-full">
      <div class="mb-2">
        <h1>Contato</h1>
      </div>

      <div class="text-justify">
        <p>Para qualquer duvida, contato, ou sugestão, entre em contato:</p>

        <div class="flex space-x-4 justify-center">
          <a
            href="https://wa.me/5511999999999"
            class="font-bold underline text-2xl"
            target="_blank"
          >
            <font-awesome-icon :icon="faWhatsapp" />
          </a>

          <a href="mailto:Jpj4h@example.com" class="font-bold underline text-2xl" target="_blank">
            <font-awesome-icon :icon="faEnvelope" />
          </a>

          <a
            href="https://www.instagram.com/maryanebedaque.di/"
            class="font-bold underline text-2xl"
            target="_blank"
          >
            <font-awesome-icon :icon="faInstagram" />
          </a>
        </div>
      </div>
    </div>
  </page>
</template>
