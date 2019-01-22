<template>
  <div class="app_wrapper">
    <appNav/>
    <div class="app_container">
      <appHeader/>
      <appHeaderTransition />
      <!-- <no-ssr placeholder="Loading..."> -->

      <appMissionStatement/>
      <!-- </no-ssr> -->
    </div>
  </div>
</template>

<script>
import Nav from '~/components/shared/Nav.vue'
import Header from '~/components/home/Header.vue'
import HeaderTransition from '~/components/home/HeaderTransition.vue'
import MissionStatement from '~/components/home/MissionStatement.vue'

export default {
  components: {
    appHeader: Header,
    appNav: Nav,
    appHeaderTransition: HeaderTransition,
    appMissionStatement: MissionStatement
  },
  methods: {
    handleScroll: function() {
      // handle the step-event as required here
      console.log("I'm in the parent")
      const [red, green, blue] = [225, 225, 225]
      const y = 0.1 + (window.scrollY || window.pageYOffset) / 100
      const [r, g, b] = [red/y, green/y, blue/y].map(Math.round)
      // console.log(this.$el.querySelector('.app_container'))
      const background = this.$el.querySelector('.app_container')
      background.style.backgroundColor = `rgb(${r}, ${g}, ${b})`
    }
  }
}
</script>

<style lang="scss">
  @import '~assets/scss/app.scss';
</style>
