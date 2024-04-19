<template>
  <div class="dont-have relative text-xl">
    <img src="/img/this-is-where-i-put-it.jpeg" alt="">
    <div class="absolute flex flex-col font-bold top-0 left-0 right-0 bottom-0">
      <div class="h-full flex flex-col justify-end">
        <div class="text-center">
          This is where I put my <slot></slot>
        </div>
      </div>
      <div class="h-full flex flex-col justify-end">
        <div class="text-center">If I have any</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.dont-have {
  text-transform: uppercase;
  -webkit-text-stroke: 3px black;
  paint-order: stroke fill;
}
</style>
