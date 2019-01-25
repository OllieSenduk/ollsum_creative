<template lang="html">
  <section class="header">
    <div class="header__title">
      <!-- <span>The</span> -->
      <h2 class="title">
       The Creative & Digital
      </h2>
      <span class="title__last"> <b>Agency</b></span>
      <div class="header__company_name">
        <b>By OLLSUM</b>
      </div>
    </div>
  </section>
</template>

<script>
export default {
}
</script>


<style lang="scss" scoped>

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

    .title__last {
      color: $secondary-color;
      font-size: 5em;
      // font-family: 'paper';
      transform: rotate(-20deg);
    }

    h2 {
      font-size: 5em;
      line-height: 90px;
      animation-duration: 3s;
    }
  }

  .header__company_name {
    text-align: right;
    margin-right: 10px;
    padding-top: 20px;
    // color: #F43565;
    font-family: 'Eina-semibold';
  }

</style>
