<template>
  <h3 class="text-4xl font-bold mt-4">Rubik Cube</h3>

  <Gallery>
    <GalleryItem src="/rubik-cube/1.jpg" alt="Solved rubik" />
    <GalleryItem src="/rubik-cube/2.jpg" alt="Shuffled rubik" />
  </Gallery>

  <hr />
  <div class="mt-2">
    Language and tool:
    <SkillIcon :size="24" icon="gradle" />
    <SkillIcon :size="24" icon="java" />
  </div>
  <hr class="my-1" />
  Source Code:
  <ProjectSourceCode name="rubik-cube" />
  <hr class="my-1" />
  Download:
  <ProjectRelease name="rubik-cube">Download (.apk)</ProjectRelease>
  <hr class="my-1" />

  <p class="mt-4">Very simple rubik cube game written in java without external library. Rendering is done using default
    opengl es 2.0 from android built-in library.
  </p>
</template>
