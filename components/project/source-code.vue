<script setup lang="ts">
defineProps<{
  name: string,
}>();
</script>

<template>
  <a target="_blank" :href="`https://github.com/yeaayy/${name}`">
    <SkillIcon :size="20" icon="github" />/{{ name }}
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
