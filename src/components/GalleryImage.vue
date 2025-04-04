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
  width: 280px;
  height: 280px;
  border-radius: 8px;
  box-shadow: 0 0 5px rgba(255, 255, 255, 0.5);
}
</style>