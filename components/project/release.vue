<script setup lang="ts">
defineProps<{
  name: string,
}>();
</script>

<template>
  <a target="_blank" :href="`https://github.com/yeaayy/${name}/releases/latest`">
    <slot>Download</slot>
  </a>
</template>

<style scoped lang="scss">
@import '../../assets/base.scss';

a {
  @apply underline decoration-white hover:bg-white;

  &:hover {
    color: $bgColor;
  }
}
</style>
