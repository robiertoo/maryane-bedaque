<script setup>
import Page from '../components/ui/Page.vue';
</script>

<template>
  <page id="about" class="space-y-4 bg-[--secondary-color]">
    <div>
      <h1>Sobre mim</h1>
  
      <div class="space-y-4 text-justify">
        <div class="md:flex space-y-4 md:space-y-0 md:space-x-4">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed sit amet nulla auctor,
            vestibulum magna sed, convallis ex. Cum sociis natoque penatibus et magnis dis parturient
            montes, nascetur ridiculus mus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            Sed sit amet nulla auctor, vestibulum magna sed, convallis ex. Cum sociis natoque
            penatibus et magnis dis parturient montes, nascetur ridiculus mus. Lorem ipsum dolor sit
            amet, consectetur adipiscing elit. Sed sit amet nulla auctor, vestibulum magna sed,
            convallis ex. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur
            ridiculus mus.
          </p>
  
          <img class="w-full md:w-1/2 rounded-3xl" src="https://picsum.photos/500/300" alt="Maryane Bedaque" />
        </div>
  
        <div class="md:flex space-y-4 md:space-y-0 md:space-x-4">
          <img
            class="w-full md:w-1/2 rounded-3xl"
            src="https://picsum.photos/500/300?"
            alt="Maryane Bedaque"
          />
  
          <p>
            Integer sed lacus sit amet nisl eleifend malesuada. Sed vitae erat auctor, aliquam massa
            ut, convallis nunc. Sed ut lorem quis nisi vestibulum dignissim. Suspendisse et nisl in
            metus malesuada ultricies. Nulla facilisi. Integer sed lacus sit amet nisl eleifend
            malesuada. Sed vitae erat auctor, aliquam massa ut, convallis nunc. Sed ut lorem quis nisi
            vestibulum dignissim. Suspendisse et nisl in metus malesuada ultricies. Nulla facilisi.
          </p>
        </div>
  
        <div class="md:flex space-y-4 md:space-y-0 md:space-x-4">
          <p>
            Integer sed lacus sit amet nisl eleifend malesuada. Sed vitae erat auctor, aliquam massa
            ut, convallis nunc. Sed ut lorem quis nisi vestibulum dignissim. Suspendisse et nisl in
            metus malesuada ultricies. Nulla facilisi.
          </p>
  
          <img
            class="w-full md:w-1/2 rounded-3xl"
            src="https://picsum.photos/500/300??"
            alt="Maryane Bedaque"
          />
        </div>
      </div>
    </div>
  </page>
</template>
