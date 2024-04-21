<template>
  <div class="galery text-center no-scrollbar">
    <slot></slot>
  </div>
</template>

<style lang="scss">
.galery {
  overflow-x: scroll;
  white-space: nowrap;
}
</style>
