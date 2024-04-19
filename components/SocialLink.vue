<script setup lang="ts">
defineProps<{
  href: string,
  icon: string,
}>();
</script>

<template>
  <a :href="href" target="_blank" class="mt-1 flex flex-row justify-items-center">
    <SkillIcon :size="24" :icon="icon" />
    <slot></slot>
  </a>
</template>
