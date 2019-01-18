<template lang="html">
  <section class="header">
    <h2 class="title">
      Creative and Digital Agency
    </h2>
    <p>Love life</p>
    <div class="svg">
    	<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 600 600" class="header__logo">
    		<rect class="path" x="100" y="150" rx="0" ry="0" width="400" height="300" stroke-width="1" stroke="black" fill="white" />
    		<rect class="path2" x="125" y="175" rx="0" ry="0" width="350" height="250" stroke-width="1" stroke="blue" fill="white" />
    		<rect class="path3" x="150" y="200" rx="0" ry="0" width="300" height="200" stroke-width="1" stroke="red" fill="white" />
    	</svg>
	</div>
  </section>
</template>

<script>
export default {
}
</script>


<style lang="scss" scoped>

  .svg {
    width: 400px;
    max-width: 100%;
    max-height: 400px;
    height: auto;
    position: absolute;
    top: 100px;
    right: -10px;

    z-index: -1;
  }

  .title {
    font-size: 6.4em
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
