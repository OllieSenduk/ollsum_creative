<template lang="html">
  <div class="menu-wrapper">
    <div class="hamburger-menu"></div>
  </div>
</template>

<script>

export default {

}
</script>

<style lang="scss">
  $bar-width: 50px;
  $bar-height: 5px;
  $bar-spacing: 10px;
  $color: pink;


.menu-wrapper {
  position: fixed;
  top: 10px;
  right: 10px;
  margin: auto;
  width: $bar-width;
  height: $bar-height + $bar-spacing*2;
  cursor: pointer;
  z-index: 10;
  }

  .hamburger-menu,
  .hamburger-menu:after,
  .hamburger-menu:before {
  width: $bar-width;
  height: $bar-height;
  }

  .hamburger-menu {
  position: relative;
  transform: translateY($bar-spacing);
  background: $color;
  transition: all 0ms 300ms;

  &.animate {
    background: $color;
  }
  }

  .hamburger-menu:before {
  content: "";
  position: absolute;
  left: 0;
  bottom: $bar-spacing;
  background: $color;
  transition: bottom 300ms 300ms cubic-bezier(0.23, 1, 0.32, 1), transform 300ms cubic-bezier(0.23, 1, 0.32, 1);
  }

  .hamburger-menu:after {
  content: "";
  position: absolute;
  left: 0;
  top: $bar-spacing;
  background: $color;
  transition: top 300ms 300ms cubic-bezier(0.23, 1, 0.32, 1), transform 300ms cubic-bezier(0.23, 1, 0.32, 1);
  }

  .hamburger-menu.animate:after {
  top: 0;
  transform: rotate(45deg);
  transition: top 300ms cubic-bezier(0.23, 1, 0.32, 1), transform 300ms 300ms cubic-bezier(0.23, 1, 0.32, 1);;
  }

  .hamburger-menu.animate:before {
  bottom: 0;
  transform: rotate(-45deg);
  transition: bottom 300ms cubic-bezier(0.23, 1, 0.32, 1), transform 300ms 300ms cubic-bezier(0.23, 1, 0.32, 1);;
  }
</style>
