<template lang="html">
  <section class="navbar">
  <!--HamBurger Icon-->
  <div class="bars " id="nav-action" v-on:click="handleNav" v-bind:class="{ active: navOpen }">
    <span class="bar"> </span>
  </div>

  <!--Navbar Links-->
  <nav id="nav" v-bind:class="{ visible: navOpen }">
    <ul>
      <li class="shape-circle circle-one"><a href="https://dribbble.com/shots/4363610-Introducing-The-Design-Genome-Project-by-InVision">Contact</a></li>
      <li class="shape-circle circle-two"><a href="#">Blog</a></li>
      <li class="shape-circle circle-three"><a href="#">Work</a></li>
      <li class="shape-circle circle-five">
        <a href="#">Home</a>
      </li>
    </ul>
  </nav>
</section>

</template>


<script>

export default {
  components: {
  },
  data: function () {
    return {
      navOpen: false
    };
  },
  methods: {
    handleNav: function() {
      var self = this
      self.navOpen = !self.navOpen
    }
  },
  mounted () {
  }
}
</script>

<style lang="scss" scoped>

// Overall Component
.navbar {
  height: 10vh;
  width: 100vw;
}
// BURGER MENU

  .bars {
    width: 27px;
    height: 27px;
    top: 30px;
    right: 30px;
    cursor: pointer;
    z-index: 101;
    padding-top:9px;
    position: fixed;
    margin-top: 10px;
    }

  .bar {
    width: 100%;
    height: 4px;
    background-color: pink;
    position: absolute;
  }

  span::before,
  span::after {
    content: "";
    display: block;
    background-color: pink;
    width: 100%;
    height: 4px;
    position: absolute;
  }

  .bar::before {
    transform: translateY(-9px);
  }

  .bar::after {
    transform: translateY(9px);
  }

  .bars.active .bar {
    background-color: transparent;
  }

  .bars.active span::before {
    animation: top-bar 1s;
    animation-fill-mode: forwards;
  }

  .bars.active span::after {
    animation: bottom-bar 1s;
    animation-fill-mode: forwards;
  }


  @keyframes top-bar {
    50% {
      transform: translateY(0);
    }
    100% {
      transform: rotate(45deg) translateY(0);
    }
  }

  @keyframes bottom-bar {
    50% {
      transform: translateY(0);
    }
    100% {
      transform: rotate(-45deg) translateY(0);
    }
  }

  /* Navbar Links CSS */

  #nav {
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    transition: all 1s;
    z-index: -1;
    overflow: hidden;
    opacity: 0;
  }

  #nav {

    a {
      color: #fff;
      text-decoration: none;
      line-height: 70vw;
      position: absolute;
      top: 40px;
      bottom: 0;
      left: 0;
      right: 0;
      text-indent: 50vw;
      border-radius: 50%;
      transition: all .5s;
    }

    a:hover {
      background: #357FFD;
    }
  }

  ul {
    list-style: none;
  }

  .visible {
    z-index: 100 !important;
    opacity: 1 !important;
  }

  .shape-circle {
    border-radius: 50%;
    width: 20vw;
    height: 20vw;
    top: -10vw;
    right: -10vw;
    position: absolute;
    transition: all 1s ease-in-out;
    background: #2979FF;
    box-shadow: 0 0px 0px rgba(4, 26, 62, 0.5);
  }

// NAV EFFECT
  nav {
    &.visible {
      li:first-child {
        width: 213vw;
        height: 213vw;
        top: -100vw;
        right: -100vw;
        z-index: 5;
        transition: all .5s ease-in-out;
        box-shadow: 0 0px 80px rgba(4, 26, 62, 0.5);
      }

      a {
        line-height: 265vw !important;
        text-indent: 15vw !important;
      }
    }

    li:nth-child(2) {
      width: 165vw;
      height: 165vw;
      top: -75vw;
      right: -75vw;
      z-index: 6;
      transition: all .6s ease-in-out;
      box-shadow: 0 0px 80px rgba(4, 26, 62, 0.5);

      a {
        line-height: 200vw !important;
        text-indent:17vw !important;
      }
    }

    li:nth-child(3){
      width: 115vw;
      height: 115vw;
      top: -50vw;
      right: -50vw;
      z-index: 7;
      transition: all .7s ease-in-out;
      box-shadow: 0 0px 80px rgba(4, 26, 62, 0.5);

      a {
        line-height: 137vw !important;
        text-indent: 17vw !important;
      }
    }

    li:last-child{
      width: 65vw;
      height: 65vw;
      top: -25vw;
      right: -25vw;
      z-index: 8;
      transition: all .8s ease-in-out;
      box-shadow: 0 0px 80px rgba(4, 26, 62, 0.5);

      a {
        line-height: 70vw !important;
        text-indent:12vw !important;
      }
    }

  }


@include mq($from: tablet) {

  #nav a {
    top: 25px;
  }

  nav {
    &.visible {
      li:first-child {
        width: 200vw;
        height: 200vw;
      }

      li:nth-child(2) {
        width: 150vw;
        height: 150vw;
      }

      li:nth-child(3){
        width: 100vw;
        height: 100vw;
      }

      li:last-child{
        width: 50vw;
        height: 50vw;
      }
    }
  }
}


</style>
