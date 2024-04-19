<script setup lang="ts">
defineProps<{
  active?: boolean,
  to?: string,
}>();
</script>

<template>
  <NuxtLink :to="to ?? ''">
    <div :class="{
    'border-t-4': $route.fullPath == to,
  }">
      <slot></slot>
    </div>
  </NuxtLink>
</template>

<style scoped lang="scss">
@import '../assets/base.scss';

div {
  @apply p-2 border-r whitespace-nowrap;
  border-top-color: lighten($bgColor, 30);
  border-right-color: lighten($bgColor, 8);

  &:hover {
    background-color: lighten($bgColor, 5);
    border-top-color: white;
    border-top-width: 4px;
  }
}
</style>
