<template>
  <div class="not-found">
    <img width="50%" class="block m-auto" src="/img/not-found.jpg"
      orignal="https://www.deviantart.com/muniversalarts/art/We-are-experiencing-Technical-Derpyculties-288304996" />
    <div class="font-bold my-2">This page is not available or still under construction.</div>
  </div>
</template>

<style scoped lang="scss">
@import '../assets/base.scss';

.not-found {
  // --tw-shadow-color: lighten($bgColor, 100);
  @apply flex flex-col text-center p-4 m-4 border border-blue-200 rounded-lg;
  box-shadow: 0 0 0.5rem lighten($bgColor, 20);
}
</style>
