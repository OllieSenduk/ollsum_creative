<template>
  <section class="wrapper">
    <appNav/>
    <appHeader/>
    <div class="container">
    </div>
  </section>
</template>

<script>
import Header from '~/components/home/Header.vue'
import Nav from '~/components/shared/Nav.vue'

export default {
  components: {
    appHeader: Header,
    appNav: Nav
  }
}
</script>

<style lang="scss">
@import '~assets/scss/app.scss';


</style>
