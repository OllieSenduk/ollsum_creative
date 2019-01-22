<template lang="html">
  <div class="navbar">


  <div id="about" class="box">
      <div class="header">
        <nav>
          <h2>
            <a href="#" onclick="">
              <video loop autoplay muted playsinline class="nav-video"  preload>
                <source src='@/assets/videos/about-19.optimized..faststart.mp4' type='video/mp4'>
              </video>
              <svg width="600" height="338" viewBox="0 0 600 338" class="svg-graphic" id="svg-graphic-about">
                <defs>
                  <mask id="about-mask" x="0" y="0" width="600" height="338" >
                    <rect x="0" y="0" width="600" height="338" fill="#fff" />
                    <polygon points="330.2,28.7 269.8,28.7 149,308.3 215.4,308.3 241.4,247.9 358.6,247.9 384.6,308.3 451,308.3  " />
                  </mask>
                </defs>
                <!-- rect should be bigger than 337.5, vector shape should be smaller than 337.5 -->
                <!-- the 337.5 is calcutated by 600 / 16 * 9 -->
                <rect x="0" y="0" width="600" height="338" />
              </svg>
              <span>About</span>
            </a>
          </h2>
        </nav>
      </div>
    </div>


    <div id="works" class="box">
      <div class="header">
        <nav>
          <h2>
            <a href="#">
              <video loop autoplay muted playsinline class="nav-video">
                <source src='@/assets/videos/works-2.optimized..faststart.mp4' type='video/mp4'>
              </video>

              <svg width="600" height="338" viewBox="0 0 600 338" class="svg-graphic" id="svg-graphic-works">
                <defs>
                  <mask id="works-mask" x="0" y="0" width="600" height="338" >
                    <rect x="0" y="0" width="600" height="338" fill="#fff" />
                    <polygon points="440.9,33.8 432.4,33.8 331.4,33.8 329.1,33.8 268.6,33.8 268.5,34.1 167.7,34.1 167.6,33.8
          102.5,33.8 196.5,303.2 241.2,303.2 299.8,115.9 358.8,303.2 403.5,303.2 497.5,33.8   "></polygon>
                  </mask>
                </defs>
                <!-- rect should be bigger than 337.5, vector shape should be smaller than 337.5 -->
                <!-- the 337.5 is calcutated by 600 / 16 * 9 -->
                <rect x="0" y="0" width="600" height="338" />
              </svg>

              <span>Works</span>
            </a>
          </h2>
        </nav>
      </div>
    </div>

    <div id="blog" class="box">
      <div class="header">
        <nav>
          <h2>
            <a href="#">
              <video loop autoplay muted playsinline class="nav-video">
                <source src='@/assets/videos/blog-8.optimized..faststart.mp4' type='video/mp4' >
              </video>

              <svg width="600" height="338" viewBox="0 0 600 338" class="svg-graphic" id="svg-graphic-blog">
                <defs>
                  <mask id="blog-mask" x="0" y="0" width="600" height="338" >
                    <rect x="0" y="0" width="600" height="338" fill="#fff" />
                    <path d="M396.2,186.5c-10.3-11.9-24.1-19.7-41.4-23.4c4.8-2.1,8.1-3.7,10-4.6c1.9-0.9,5.2-3.3,10-7c14.1-10.7,21.2-26.9,21.2-48.8
          c0-18.1-6.3-34.4-18.8-48.8c-6.9-7.7-17.3-13.9-31-18.4c-13.7-4.5-30.1-6.8-49-6.8H188.4v279.6h122.4c38.4,0,65.3-8.7,80.8-26
          c13.3-14.9,20-32.1,20-51.6C411.6,213.1,406.5,198.4,396.2,186.5z" />
                  </mask>
                </defs>
                <!-- rect should be bigger than 337.5, vector shape should be smaller than 337.5 -->
                <!-- the 337.5 is calcutated by 600 / 16 * 9 -->
                <rect x="0" y="0" width="600" height="338" />
              </svg>

              <span>Blog</span>
            </a>
          </h2>
        </nav>
      </div>
    </div>



    <div id="contact" class="box">
      <div class="header">
        <nav>
          <h2>
            <a href="#">
              <video loop autoplay muted playsinline class="nav-video">
                <source src='@/assets/videos/contact-3.optimized..faststart.mp4' type='video/mp4' >
              </video>
              <svg width="600" height="338" viewBox="0 0 600 338" class="svg-graphic" id="svg-graphic-contact">
                <defs>
                  <mask id="contact-mask" x="0" y="0" width="600" height="338" >
                    <rect x="0" y="0" width="600" height="338" fill="#fff" />
                    <path d="M297.1,306c-75.8,0-137.5-61.7-137.5-137.5S221.3,31,297.1,31c49.2,0,94.9,26.5,119.3,69.2l-120,67.9l119.1,70.2
          c-11.9,20.2-28.9,37.1-49.1,48.9C345.6,299.5,321.5,306,297.1,306z" />
                  </mask>
                </defs>
                <!-- rect should be bigger than 337.5, vector shape should be smaller than 337.5 -->
                <!-- the 337.5 is calcutated by 600 / 16 * 9 -->
                <rect x="0" y="0" width="600" height="338" />
              </svg>
              <span>Contact</span>
            </a>
          </h2>
        </nav>
      </div>


    </div>



  </div>




</template>

<script>
export default {
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
}
</script>

<style lang="css">

/* home and nav */
.box {
  width: 50%;
  height: 50%;
  display: block;
  position: absolute;
  overflow: hidden; }

#about {
  left: 0;
  top: 0; }
  #about .header {
    background: #fff; }

#works {
  right: 0;
  top: 0; }
  #works .header {
    background: #f5f5f5; }

#blog {
  left: 0;
  bottom: 0; }
  #blog .header {
    background: #f5f5f5; }

#contact {
  right: 0;
  bottom: 0; }
  #contact .header {
    background: #e9e9e9; }

.header {
  width: 100%;
  height: 100%;
  overflow: hidden; }

.header nav {
  width: 100%;
  height: 100%; }

.header nav h2 {
  width: 100%;
  height: 100%;
  margin: 0; }

.header a {
  display: block;
  width: 100%;
  height: 100%;
  padding: 20px;
  position: relative; }

.header span {
  position: absolute;
  z-index: 10;
  display: inline-block;
  bottom: 30%;
  font-size: 20px;
  color: #000;
  text-transform: uppercase;
  font-weight: 700;
  font-family: montserrat;
  line-height: 1em;
  transition-property: left;
  transition-duration: .3s; }

#about .header span {
  left: 60%; }

#works .header span {
  left: 58%; }

#blog .header span {
  left: 57%; }

#contact .header span {
  left: 56%; }

.header .title span.c {
  letter-spacing: -30px; }

.header .title span.w {
  letter-spacing: -140px; }

.header .title span.b {
  letter-spacing: -45px; }

.color-overlay {
  width: 100%;
  height: 100%;
  display: block;
  position: absolute;
  left: 0;
  top: 0;
  z-index: 2;
  opacity: 1;
  transition-property: opacity;
  transition-duration: 0.1s; }

.color-overlay.orange {
  background-color: rgba(245, 104, 35, 0.9); }

.color-overlay.green {
  background-color: rgba(38, 165, 86, 0.9); }

.dark-overlay {
  width: 100%;
  height: 100%;
  display: block;
  display: none;
  position: absolute;
  left: 0;
  top: 0;
  z-index: 2;
  background-color: rgba(0, 0, 0, 0.85);
  opacity: 1;
  transition-property: opacity;
  transition-duration: 0.1s; }

.header:hover .title {
  opacity: 0.2;
  left: -20%;
  transition-property: all;
  transition-duration: 0.3s;
  transition-timing-function: ease-in; }

.header:hover .dark-overlay, .header:hover .color-overlay {
  opacity: 0;
  transition-property: opacity;
  transition-duration: 0.2s; }

#back {
  position: fixed;
  color: #000;
  z-index: 3;
  top: 10px;
  right: 25px;
  font-size: 36px;
  line-height: 36px;
  padding: 20px;
  -webkit-tap-highlight-color: transparent; }

#back:hover {
  transform: rotate(360deg);
  transition-property: transform;
  transition-duration: 0.6s;
  transition-timing-function: ease; }

svg path, svg polygon {
  transform: scale(0.9);
  transform-origin: center;
  transition-property: transform;
  transition-duration: .3s; }

body.hover-about svg #svg-about path, body.hover-about svg #svg-about polygon,
body.hover-works svg #svg-works path, body.hover-works svg #svg-works polygon,
body.hover-blog svg #svg-blog path, body.hover-blog svg #svg-blog polygon,
body.hover-contact svg #svg-contact path, body.hover-contact svg #svg-contact polygon {
  transform: scale(1.2);
  transform-origin: center;
  transition-property: transform;
  transition-duration: .3s; }

.box:hover .header span {
  bottom: 30%;
  transition-property: left;
  transition-duration: .3s; }

#about:hover .header span {
  left: 70%; }

#works:hover .header span {
  left: 68%; }

#blog:hover .header span {
  left: 67%; }

#contact:hover .header span {
  left: 67%; }

.header:hover .nav-video {
  filter: none; }

svg #svg-about .path {
  transform-origin: center;
  transition-property: transform;
  transition-duration: .3s; }

.header svg {
  position: static;
  display: block;
  transform: none;
  z-index: 3;
  opacity: 1;
  transition: none;
  transform-origin: center;
  display: block;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate3d(-50%, -50%, 0) scale(1.01);
  margin: 0;
  z-index: 2; }

svg#svg-graphic-about > rect {
  -webkit-mask: url(#about-mask);
  mask: url(#about-mask);
  fill: #fff; }

svg#svg-graphic-about .path {
  transform: scale(1);
  transform-origin: center;
  fill: #000; }

svg#svg-graphic-works > rect {
  -webkit-mask: url(#works-mask);
  mask: url(#works-mask);
  fill: #f5f5f5; }

svg#svg-graphic-works .path {
  transform: scale(1);
  transform-origin: center;
  fill: #000; }

svg#svg-graphic-blog > rect {
  -webkit-mask: url(#blog-mask);
  mask: url(#blog-mask);
  fill: #f5f5f5; }

svg#svg-graphic-blog .path {
  transform: scale(1);
  transform-origin: center;
  fill: #000; }

svg#svg-graphic-contact > rect {
  -webkit-mask: url(#contact-mask);
  mask: url(#contact-mask);
  fill: #e9e9e9; }

svg#svg-graphic-contact .path {
  transform: scale(1);
  transform-origin: center;
  fill: #000; }

body > svg {
  display: none; }

/* content */
.invisible {
  visibility: hidden; }

.box {
  transition-duration: .3s;
  transition-timing-function: ease-out;
  -webkit-tap-highlight-color: transparent; }

.box.inactive-w-0 {
  width: 0; }

.box.inactive-h-0 {
  height: 0; }

.box.inactive-h-w-0 {
  width: 0;
  height: 0; }

.nav-video {
  width: 600px;
  height: auto;
  display: block;
  object-fit: cover;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate3d(-50%, -50%, 0);
  margin: 0;
  filter: contrast(110%) brightness(103%); }

.box.active {
  transition-timing-function: ease-in;
  width: 100%;
  height: 100%;
  padding: 80px 20px 20px;
  overflow-y: hidden;
  -webkit-overflow-scrolling: touch; }
  .box.active .header-title {
    visibility: visible;
    position: absolute;
    top: 40%;
    left: 10%;
    z-index: 2;
    padding-right: 10%;
    color: #fff; }
    .box.active .header-title h2 {
      font-size: 60px;
      font-family: montserrat;
      margin-bottom: 40px; }
    .box.active .header-title p {
      font-size: 24px;
      margin-bottom: 40px;
      line-height: 1.3em; }
  .box.active .content {
    visibility: visible; }
  .box.active .dark-overlay {
    display: none; }
  .box.active .header a {
    cursor: default;
    overflow: hidden; }
  .box.active .header h2 {
    overflow: hidden; }
  .box.active .header {
    position: relative;
    width: 100%;
    overflow: visible; }
  .box.active .header span {
    display: none; }
  .box.active .nav-video {
    transition: none; }

#about.box.active svg, #works.box.active svg, #blog.box.active svg, #contact.box.active svg {
  display: none; }

#about.box.active .nav-video, #works.box.active .nav-video, #blog.box.active .nav-video, #contact.box.active .nav-video {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate3d(-50%, -50%, 0);
  margin: 0;
  filter: none; }

.colored-title {
  color: #ff5242; }

.big-text {
  font-size: 24px;
  line-height: 1.9em; }

  svg path, svg polygon {
    transform: scale(0.5);
    transform-origin: center;
    transition-property: transform;
    transition-duration: .3s; }


</style>
