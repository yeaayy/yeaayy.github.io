<script setup lang="ts">
import type Data from './data';

defineProps<{
  src: string,
  alt?: string,
}>();

const parent = inject<Data>('gallery')!!;

parent.queue();

function load() {
  parent.load();
}
</script>

<template>
  <div :style="alt ? `--alt:'${alt}'` : null">
    <NuxtImg :src="`/img/${src}`" @load="load" @error="load" :alt="alt" :title="alt" />
  </div>
</template>

<style scoped lang="scss">
div {
  @apply text-sm inline-block text-center mx-1 my-auto max-w-[100%];
  scroll-snap-align: center;
  scroll-snap-stop: normal;

  &::after {
    content: var(--alt);
  }

  img {
    margin: auto;
    max-height: 24rem;
    max-width: -moz-available;
  }
}
</style>
