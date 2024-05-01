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
