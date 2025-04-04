<script setup>

import GalleryImage from "@/components/GalleryImage.vue";
import { reactive } from 'vue';

const images = reactive([]);
for (let i=0; i < 16; i++) {
  images.push({
    id: i,
    url: `https://picsum.photos/400/400?random=${Math.random()}`,
  });
}
</script>

<template>
  <h3>
    Gallery
  </h3>
  <div class="grid-container">
    <GalleryImage v-for="image in images" :image="image" :key="image.id" />
  </div>
</template>

<style scoped>
  .grid-container {
    height: 1200px;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr 1fr;
    justify-items: center;
    align-items: center;
    margin-bottom: 3rem;
  }
</style>