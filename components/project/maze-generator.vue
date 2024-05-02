<template>
  <h3 class="text-4xl font-bold mt-4">Maze Generator</h3>

  <Gallery>
    <GalleryItem src="/maze-generator/1.png" alt="Preview on desktop" />
    <GalleryItem src="/maze-generator/2.png" alt="Preview on desktop" />
    <GalleryItem src="/maze-generator/3.png" alt="Preview on mobile" />
    <GalleryItem src="/maze-generator/4.png" alt="Preview on mobile" />
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
  <ProjectSourceCode name="maze-generator" />
  <hr class="my-1" />
  Demo:
  <ProjectPreview name="maze-generator" />
  <hr class="my-1" />

  <p class="mt-4">Simple tree based maze generator with adjustable size.</p>

  <p class="mt-4">The algorithm to generate this is very simple:</p>
  <ol class="list-decimal pl-4">
    <li class="list-item">Pick starting point.</li>
    <li class="list-item">Move randomly, but don't visit tile that already visited.</li>
    <li class="list-item">If all neighboring tile already visited take goto previous tile then repeat step 2.</li>
    <li class="list-item">Repeat step above until all tile is visited.</li>
  </ol>

  <p class="mt-4">To generate the solution is also easy. Starting from destination tile then go to it's parents tile
    until you get back to the starting point. This work because all tile have parent that will eventualy lead to the
    starting point.</p>
</template>
