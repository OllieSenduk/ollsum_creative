<template>
  <section class="wrapper">
    <appNav/>
    <appHeader/>
    <div class="container">
    </div>
  </section>
</template>

<script>
import Nav from '~/components/shared/Nav.vue'
import Header from '~/components/home/Header.vue'
import LogoTransition from '~/components/home/LogoTransition.vue'

export default {
  components: {
    appHeader: Header,
    appNav: Nav,
    appLogoTransition: LogoTransition
  }
}
</script>

<style lang="scss">
  @import '~assets/scss/app.scss';
</style>
