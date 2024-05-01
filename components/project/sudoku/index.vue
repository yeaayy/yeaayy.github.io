<script setup lang="ts">
</script>

<template>
  <h3 class="text-4xl font-bold mt-4">Sudoku Solver</h3>

  <Gallery>
    <GalleryItem src="/sudoku/input1.png" alt="Simple 3x3 sudoku input" />
    <GalleryItem src="/sudoku/output1.png" alt="The solution" />
    <GalleryItem src="/sudoku/input2.png" alt="More complex sudoku input" />
    <GalleryItem src="/sudoku/output2.png" alt="The solution" />
  </Gallery>

  <hr />
  <div class="mt-2">
    Language and tool:
    <SkillIcon :size="24" icon="cpp" />
    <SkillIcon :size="24" icon="cmake" />
  </div>
  <hr class="my-1" />
  Source Code:
  <ProjectSourceCode name="sudoku" />
  <hr class="my-1" />

  <p class="mt-4">Tool to solve 3x3 sudoku with easily customizable rule and board shape.</p>

  <p class="mt-4">But, currently you need to edit the source code to to get customized rule and board shape.</p>
</template>
