<script setup lang="ts">
</script>

<template>
  <h3 class="text-4xl font-bold mt-4">2048</h3>

  <Galery>
    <GaleryItem src="/2048/ss-desktop.png" alt="View in desktop" />
    <GaleryItem src="/2048/ss-mobile.png" alt="View in mobile" />
    <GaleryItem src="/2048/ss-play.png" alt="Play mode option" />
    <GaleryItem src="/2048/ss-replay.png" alt="Replay mode option" />
    <GaleryItem src="/2048/ss-random.png" alt="Random mode option" />
  </Galery>

  <hr />
  <div class="mt-2">
    Language and tool:
    <SkillIcon :size="24" icon="html" alt="HTML" />
    <SkillIcon :size="24" icon="css" alt="CSS" />
    <SkillIcon :size="24" icon="js" alt="Javascript" />
  </div>
  <hr class="mt-1" />

  <p class="mt-4">Just normal 2048 game. But to make it a bit different I add seed and game mode. When using seed the
    game will spawn the new tile at exactly the same position if the player using the same movement. </p>

  <ul class="list-disc ml-4 mt-2">
    <li class="list-item">Play mode: Normal game play.</li>
    <li class="list-item">Replay mode: as it's name suggest it's replay the game from history.</li>
    <li class="list-item">Random mode: the bot will give random move using bot seed.</li>
  </ul>

  <p class="mt-2">The game has to be reseted to in order to change game mode.</p>
</template>
