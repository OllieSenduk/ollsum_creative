<template lang="html">
  <section class="header_transition">
    <div id="transition_component">
      <div class="header__svg" >
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 600 600" class="header__logo">
          <rect class="path" x="100" y="150" rx="0" ry="0" width="400" height="300" stroke-width="1" stroke="black" fill="white" />
          <rect class="path2" x="125" y="175" rx="0" ry="0" width="350" height="250" stroke-width="1" stroke="blue" fill="white" />
          <rect class="path3" x="150" y="200" rx="0" ry="0" width="300" height="200" stroke-width="1" stroke="red" fill="white" />
        </svg>
      </div>
  </div>
</section>

</template>


<script>

export default {
  data: function() {
    return {
      changeColor: false,
      elementHeightStart: "",
      elementHeightEnd: "",
      element: ""
    }
  },
  methods: {
    // handleScroll: function() {
    //   if ((window.scrollY >= this.elementHeightStart) && (window.scrollY <= this.elementHeightEnd)) {
    //     const [red, green, blue] = [69, 111, 225]
    //     const y = 1 + (window.scrollY || window.pageYOffset) / 150
    //     const [r, g, b] = [red/y, green/y, blue/y].map(Math.round)
    //     this.element.style.backgroundColor = `rgb(${r}, ${g}, ${b})`
    //   }
    // }
  },
  // mounted() {
  //   this.element = this.$el.querySelector('#transition_component')
  //   this.elementHeightStart = this.element.getBoundingClientRect().top + window.scrollY;
  //   this.elementHeightEnd = this.element.getBoundingClientRect().bottom + window.scrollY;
  //   console.log(this.elementHeightEnd)
  //
  //     window.addEventListener('scroll', () => {
  //         // this.$parent.handleScroll();
  //
  //         const [red, green, blue] = [225, 225, 225]
  //         const y = 0.2 + (window.scrollY || window.pageYOffset) / 300
  //         const [r, g, b] = [red/y, green/y, blue/y].map(Math.round)
  //         const hello = this.$el.querySelector('.wrapper')
  //         // this.element.style.backgroundColor = `rgb(${r}, ${g}, ${b})`
  //     });
  //   }
}
</script>


<style lang="scss" scoped>

#transition_component {
  // background-color: pink;
  height: 200vh;
  width: 100vw;
}

.header__svg {
  transform: rotate(-20deg);
  // background-color: pink;
  border-radius: 5px;
}

.path {
  stroke-dasharray: 2000;
  stroke-dashoffset: 2000;
  animation: dash 2s linear forwards;
}

.path2 {
  stroke-dasharray: 3000;
  stroke-dashoffset: 2000;
  animation: dash 4s linear forwards;
}

.path3 {
  stroke-dasharray: 1000;
  stroke-dashoffset: 1000;
  animation: dash 3s linear forwards;
}

@keyframes dash {
  to {
    stroke-dashoffset: 0;
  }
}


</style>
