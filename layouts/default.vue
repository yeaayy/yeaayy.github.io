<script setup lang="ts">
</script>

<template>
  <Navbar />

  <div class="content">
    <div>
      <slot />
    </div>

    <div>
      <MyFav />
    </div>
  </div>
</template>

<style scoped lang="scss">
.content {
  @apply flex flex-col md:flex-row md:mt-6;

  >* {
    @apply mx-4 mb-8;
  }

  > :first-child {
    @apply md:w-[33rem] lg:w-[45rem] md:ml-auto;
  }

  > :last-child {
    @apply md:w-[11rem] lg:w-[15rem] md:mr-auto;
  }
}
</style>
