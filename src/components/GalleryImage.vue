<script setup>
import { ref, defineProps } from 'vue';
  const props = defineProps({
    image: {
      type: Object,
      required: true,
    }
  });

  const imageStyle = ref({
    backgroundImage: `url(${props.image.url})`,
    backgroundSize: 'cover',
    backgroundPosition: 'center',
  });

</script>

<template>
<div :style="imageStyle"></div>
</template>

<style scoped>
div {
  width: 90%;
  aspect-ratio: 1/1;
  border-radius: 8px;
  box-shadow: 0 0 5px rgba(255, 255, 255, 0.5);
  transition: transform 0.3s ease;
}

div:hover {
  transform: scale(1.1);
  box-shadow: 0 0 10px rgba(255, 255, 255, 0.7);
}

</style>