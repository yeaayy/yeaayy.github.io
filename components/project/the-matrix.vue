<template>
  <h3 class="text-4xl font-bold mt-4">The Matrix</h3>

  <Gallery>
    <GalleryItem src="/the-matrix.png" alt="Preview" />
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
  <ProjectSourceCode name="the-matrix" />
  <hr class="my-1" />
  Demo:
  <ProjectPreview name="the-matrix" />
  <hr class="my-1" />

  <p class="mt-4">The matrix styled text waterfall wallpaper/screensaver.</p>
</template>
