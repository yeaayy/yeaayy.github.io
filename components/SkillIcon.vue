<script setup lang="ts">
defineProps<{
  icon: string,
  alt?: string,
  size?: number,
}>();

function getUrl(name: string) {
  const local: any = {
    'facebook': 'svg',
  };
  if (name in local) {
    return `/img/${name}.${local[name]}`;
  } else {
    return `https://skillicons.dev/icons?i=${name}&theme=light`;
  }
}
</script>

<template>
  <img class="inline-block mx-1" :src="getUrl(icon)" :width="`${size ?? 36}px`" :alt="alt" :title="alt">
</template>
