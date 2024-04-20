<script setup lang="ts">
defineProps<{
  to?: string,
}>();
</script>

<template>
  <NuxtLink :to="to ?? ''">
    <div :class="{
    'active': $route.fullPath == to,
  }">
      <slot></slot>
    </div>
  </NuxtLink>
</template>

<style scoped lang="scss">
@import '../assets/base.scss';

div {
  @apply p-2 border-r border-l whitespace-nowrap border-t-4;
  border-top-color: transparent;
  border-left-color: lighten($bgColor, 8);
  border-right-color: lighten($bgColor, 8);

  &.active {
    border-top-color: lighten($bgColor, 30);
  }

  &:hover {
    background-color: lighten($bgColor, 5);
    border-top-color: white;
  }
}
</style>
