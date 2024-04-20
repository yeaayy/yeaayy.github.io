<script setup lang="ts">
defineProps<{
  src: string,
  alt?: string,
}>();
</script>

<template>
  <div>
    <NuxtImg :src="`/img/${src}`" :alt="alt" :title="alt" />
    {{ alt }}
  </div>
</template>

<style scoped lang="scss">
div {
  @apply text-sm inline-block text-center mx-1;

  img {
    height: 24rem;
  }
}
</style>
