<script setup lang="ts">
</script>

<template>
  <h3 class="text-3xl font-bold mt-4">Clone of game Townsmen</h3>

  <Gallery>
    <GalleryItem src="/gm/ss1.jpg" alt="Character chopping wood, render error" />
    <GalleryItem src="/gm/ss2.jpg" alt="Castle, water" />
    <GalleryItem src="/gm/ss3.jpg" alt="Terrain editor" />
  </Gallery>

  <hr />
  <div class="mt-2">
    Language and tool:
    <SkillIcon :size="24" icon="cpp" alt="C++" />
    <SkillIcon :size="24" icon="cmake" alt="CMake" />
  </div>
  <hr class="my-1" />
  Source Code:
  <ProjectSourceCode name="gm" />
  <hr class="my-1" />

  <p class="mt-4">This is probably the bigest project that I made by myself. I made this because I want to start in game
    development but I don't have any game idea so I just tought "Why don't just make copy of game that I play" and here
    is the result.</p>

  <p class="mt-2">I start this project using typescript because it type safe and doesn't require much time to compile.
    But later it quickly running into performance issue. At this point the game is not yet playable and dont have any
    animation yet, just bunch of image moving.</p>

  <p class="mt-2">Later I migrate all the code into C++ and use "make" to build the project. Then I add animation,
    and give routine to the character so they can move and do activity automaticly just like in the original game.</p>

  <p class="mt-2">I separate this project into few smaller project so I can use them in other project. Because of that
    using "make" to build the project is a nightmare for this project, because I have to each file depedency manually. I
    made little script to do track the dependency but it hard to maintain. So recently (14 Apr 2024) I change the build
    tool to cmake. It's quicker to setup and easier to maintain.</p>

  <p class="mt-2">As 20 April 2024 this project is not finished yet. All basic game mechanic is finished. I just have to
    fix minor rendering error, add more character behaviour, make the UI and the game will be completed.</p>

</template>
