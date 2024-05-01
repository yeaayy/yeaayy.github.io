<script setup lang="ts">
import type Data from './data';

const container = ref<HTMLDivElement>() as Ref<HTMLDivElement>;
const overflow = ref(false);
const count = ref(0);

provide<Data>('gallery', {
  queue,
  load,
});

watch(count, (val) => {
  if (val === 0) recalculate();
});

function queue() {
  count.value++;
}

function load() {
  count.value--;
}

function recalculate() {
  overflow.value = container.value.scrollWidth > container.value.clientWidth;
}

function prevImage() {
  container.value.scrollBy({ left: -100, behavior: 'smooth' })
}

function nextImage() {
  container.value.scrollBy({ left: 100, behavior: 'smooth' })
}

onMounted(() => {
  window.addEventListener('resize', recalculate);
});

onBeforeUnmount(() => {
  window.removeEventListener('resize', recalculate);
})
</script>

<template>
  <div class="gallery">
    <div class="no-scrollbar" ref="container">
      <slot></slot>
    </div>
    <div class="prev" @click="prevImage" v-if="overflow"></div>
    <div class="next" @click="nextImage" v-if="overflow"></div>
  </div>
</template>

<style lang="scss">
.gallery {
  @apply text-center relative justify-items-center;

  > :first-child {
    @apply flex overflow-x-scroll;
    scroll-snap-type: x mandatory;

    > :first-child {
      @apply ml-auto;
    }

    > :last-child {
      @apply mr-auto;
    }
  }

  .next,
  .prev {
    @apply absolute top-0 bottom-0 w-24 bg-white bg-opacity-30 opacity-40 hover:opacity-80;
  }

  .prev {
    @apply left-0;
  }

  .next {
    @apply right-0;
  }
}
</style>
