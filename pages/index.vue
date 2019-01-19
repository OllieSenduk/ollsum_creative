<template>
  <section class="wrapper">
      <appNav/>
      <div class="app_container">
        <appHeader/>
      </div>
      <appLogoTransition />
      <appMissionStatement/>
    </div>
  </section>
</template>

<script>
import Nav from '~/components/shared/Nav.vue'
import Header from '~/components/home/Header.vue'
import LogoTransition from '~/components/home/LogoTransition.vue'
import MissionStatement from '~/components/home/MissionStatement.vue'

export default {
  components: {
    appHeader: Header,
    appNav: Nav,
    appLogoTransition: LogoTransition,
    appMissionStatement: MissionStatement
  },
  methods: {
    handleScroll: function() {
      // handle the step-event as required here
      console.log("hello")
    }
  }
}
</script>

<style lang="scss">
  @import '~assets/scss/app.scss';
</style>
