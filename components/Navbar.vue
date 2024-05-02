<template>
  <div id="navbar">
    <div class="no-scrollbar">
      <NavItem to="/">Main</NavItem>
      <NavItem to="/about">More About Me</NavItem>
      <NavItem to="/game-projects">Game Projects</NavItem>
      <NavItem to="/tools">My Tools</NavItem>
      <NavItem to="/other-projects">Other Projects</NavItem>
      <NavItem to="/3d">3D Render</NavItem>
      <NavItem to="/vector">2D Vector</NavItem>
      <NavItem to="/drawing">Drawing</NavItem>
    </div>
  </div>
</template>

<style lang="scss">
#navbar {
  >* {
    @apply mx-auto px-4 md:max-w-[48rem] lg:max-w-[64rem];
    @apply flex overflow-x-scroll;

    :first-child {
      @apply ml-auto
    }

    :last-child {
      @apply mr-auto
    }
  }
}
</style>
