<template>
  <h3 class="text-4xl font-bold mt-4">Random Yu-Gi-Oh! card</h3>

  <Gallery>
    <GalleryItem src="/random-yugioh-card/1.png" alt="Mobile view" />
    <GalleryItem src="/random-yugioh-card/2.png" alt="Desktop view" />
  </Gallery>

  <hr />
  <div class="mt-2">
    Language and tool:
    <SkillIcon :size="24" icon="html" />
    <SkillIcon :size="24" icon="css" />
    <SkillIcon :size="24" icon="javascript" />
  </div>
  <hr class="my-1" />
  Source Code:
  <ProjectSourceCode name="random-yugioh-card" />
  <hr class="my-1" />
  Demo:
  <ProjectPreview name="random-yugioh-card" />
  <hr class="my-1" />

  <p class="mt-4">Just an infinitely scrollable random Yu-Gi-Oh! card.</p>
</template>
