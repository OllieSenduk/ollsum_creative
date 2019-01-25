<template>
  <div class="app_wrapper">
    <appHamburger v-on:navClicked="handleNav" />
    <appNavigation/>
    <div class="app_background">
      <div class="app_container">

        <appHeader/>
        <appHeaderTransition />
        <appMissionStatement/>

      </div>
    </div>
  </div>
</template>

<script>
import Nav from '~/components/shared/Nav.vue'
import Navigation from '~/components/shared/Navigation.vue'
import Hamburger from '~/components/shared/Hamburger.vue'
import Header from '~/components/home/Header.vue'
import HeaderTransition from '~/components/home/HeaderTransition.vue'
import MissionStatement from '~/components/home/MissionStatement.vue'

export default {
  components: {
    appHeader: Header,
    appHamburger: Hamburger,
    appNav: Nav,
    appNavigation: Navigation,
    appHeaderTransition: HeaderTransition,
    appMissionStatement: MissionStatement
  },
  methods: {
    handleScroll: function() {
      const [red, green, blue] = [225, 225, 225]
      const y = 0.1 + (window.scrollY || window.pageYOffset) / 50
      const [r, g, b] = [red/y, green/y, blue/y].map(Math.round)
      const background = this.$el.querySelector('.app_background')
      background.style.backgroundColor = `rgb(${r}, ${g}, ${b})`
    },
    handleNav: function() {
      console.log("nav handled")
    }
  },
  mounted() {
    var self = this
    window.addEventListener('scroll', () => {
      self.handleScroll()
    })
  }
}
</script>

<style lang="scss" scoped>
  @import '~assets/scss/app.scss';
</style>
