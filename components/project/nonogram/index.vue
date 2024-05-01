<script setup lang="ts">
</script>

<template>
  <h3 class="text-4xl font-bold mt-4">Nonogram Solver</h3>

  <Gallery>
    <GalleryItem src="/nonogram/input1.png" alt="Simple nonogram input" />
    <GalleryItem src="/nonogram/output1.png" alt="The solution" />
  </Gallery>

  <hr />
  <div class="mt-2">
    Language and tool:
    <SkillIcon :size="24" icon="cpp" />
    <SkillIcon :size="24" icon="cmake" />
  </div>
  <hr class="my-1" />
  Source Code:
  <ProjectSourceCode name="nonogram" />
  <hr class="my-1" />

  <p class="mt-4">Tool to solve nonogram puzzle. The implementation use brute force method with very little
    optimization, so tool can't solve large puzzle. Other limitation include:</p>
  <ul class="list-disc pl-4">
    <li class="list-item">Can't solve nonogram that require some trial and error.</li>
    <li class="list-item">There is no error message if the input formated incorrectly.</li>
  </ul>
</template>
