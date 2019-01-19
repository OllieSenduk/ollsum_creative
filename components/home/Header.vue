<template lang="html">
  <section class="header">
    <div class="header__title">
      <h2 class="title">
        Creative and Digital Studio
      </h2>
    </div>
  </section>
</template>

<script>
export default {
}
</script>


<style lang="scss" scoped>

  .header {
    height: 90vh;
  }


  .header__svg {
    width: 400px;
    max-width: 100%;
    max-height: 400px;
    height: auto;
    position: absolute;
    bottom: 10px;
    right: -10px;

    z-index: -1;
  }

  .header__title {

    h2 {
    font-size: 6.4em
    }
  }

</style>
