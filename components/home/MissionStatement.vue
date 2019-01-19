<template lang="html">
  <section class="mission_statement">
    <div class="title">
      <h2>Think.
        <br>
        Do.
        <br>
        Propagate.</h2>
    </div>
    <div class="vimeo-wrapper">
      <iframe src="https://player.vimeo.com/video/76979871?background=1&autoplay=1&loop=1&byline=0&title=0"
           frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
    </div>
  </section>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
  .mission_statement {
    background-color: black;
    height: 90vh;

    color: white;
  }

  .vimeo-wrapper {
   position: relative;
   top: 0;
   left: 0;
   width: 100%;
   height: 100%;
   z-index: 2;
   pointer-events: none;
   overflow: hidden;
  }
  .vimeo-wrapper iframe {
     width: 100vw;
     height: 56.25vw; /* Given a 16:9 aspect ratio, 9/16*100 = 56.25 */
     min-height: 100vh;
     min-width: 177.77vh; /* Given a 16:9 aspect ratio, 16/9*100 = 177.77 */
     position: absolute;
     top: 50%;
     left: 50%;
     transform: translate(-50%, -50%);
  }
</style>
