<script setup lang="ts">
</script>

<template>
  <Navbar />

  <div class="flex flex-col md:flex-row md:mt-6 md:px-48">
    <div class="mx-4 flex-[4] mb-8">
      <slot />
    </div>

    <div class="mx-4 flex-[1] mb-8">
      <MyFav />
    </div>
  </div>
</template>
