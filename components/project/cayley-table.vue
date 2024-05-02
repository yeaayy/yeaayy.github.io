<template>
  <h3 class="text-4xl font-bold mt-4">Cayley Table Generator</h3>

  <Gallery>
    <GalleryItem src="/cayley-table/1.jpg" alt="Preview on mobile" />
    <GalleryItem src="/cayley-table/2.png" alt="Preview on desktop" />
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
  <ProjectSourceCode name="cayley-table" />
  <hr class="my-1" />
  Demo:
  <ProjectPreview name="cayley-table" />
  <hr class="my-1" />

  <p class="mt-4">This tool used to generate cayley table from permutation matrix. The tool will add new matrix when
    necessary and automaticaly give a label to the new matrix. The automatic labeling use alphabetical order, currently
    only latin alphabet are supported. The inputed matrix could be copy as json and a json could be pasted to fill the
    permutation matrix.
  </p>
</template>
