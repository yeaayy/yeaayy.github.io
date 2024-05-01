<script setup lang="ts">
defineProps<{
  name: string,
}>();
</script>

<template>
  <a target="_blank" :href="`https://yeaayy.github.io/${name}`">Try out in new tab</a>
</template>

<style scoped lang="scss">
@import '../../assets/base.scss';

a {
  @apply border p-1 m-1 rounded-md;
  border-color: lighten($bgColor, 30);

  &:hover {
    border-color: lighten($bgColor, 50);
    background-color: lighten($bgColor, 20);
  }
}
</style>
