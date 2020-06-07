<template>
  <div class="wrapper" id="projects">
    <div class="projects">
      <hooper :settings="hooperSettings">
        <slide :index="0">
          <div class="block-wrapper">
            <img src="../assets/website.jpg" alt="" class="block-" />
            <div class="block-info-content">
              <p class="title-project">Website</p>
              <p class="info-about-project">
                This is the site you looking now. I'm using Vue.js, Stylus.
              </p>
              <a
                href="https://github.com/georginklv/website"
                target="_blank"
                class="gitHub-link"
              >
                <img
                  src="../assets/github-black.webp"
                  alt=""
                  class="gitHub-logo"
                />
                <p class="github">GitHub</p>
              </a>
            </div>
          </div>
        </slide>

        <slide :index="1">
          <div class="block-wrapper">
            <img src="../assets/calculator.png" alt="" class="block-" />
            <div class="block-info-content">
              <p class="title-project">Vue Calculator</p>
              <p class="info-about-project">Calcutor made with Vue.js</p>
              <a
                href="https://github.com/georginklv/vue-calculator"
                target="_blank"
                class="gitHub-link"
              >
                <img
                  src="../assets/github-black.webp"
                  alt=""
                  class="gitHub-logo"
                />
                <p class="github">GitHub</p>
              </a>
            </div>
          </div>
        </slide>

        <slide :index="2">
          <div class="block-wrapper">
            <img src="../assets/flappy.jpg" alt="" class="block-" />
            <div class="block-info-content">
              <p class="title-project">letqshtoPile</p>
              <p class="info-about-project">
                This is remake of the famous game Flappy Bird. I'm using only
                JavaScript, HTML5, CSS3. Still in progres ...
              </p>
              <a
                href="https://github.com/georginklv/lqtqshtoPile"
                target="_blank"
                class="gitHub-link"
              >
                <img
                  src="../assets/github-black.webp"
                  alt=""
                  class="gitHub-logo"
                />
                <p class="github">GitHub</p>
              </a>
            </div>
          </div>
        </slide>

        <slide :index="3">
          <div class="block-wrapper">
            <img src="../assets/weather.jpg" alt="" class="block-" />
            <div class="block-info-content">
              <p class="title-project">Vue Weather</p>
              <p class="info-about-project">Weather app made with Vue.js</p>
              <a
                href="https://github.com/georginklv/vue-weather"
                target="_blank"
                class="gitHub-link"
              >
                <img
                  src="../assets/github-black.webp"
                  alt=""
                  class="gitHub-logo"
                />
                <p class="github">GitHub</p>
              </a>
            </div>
          </div>
        </slide>
      </hooper>
    </div>
  </div>
</template>

<script>
import { Hooper, Slide } from "hooper";
import "hooper/dist/hooper.css";

export default {
  name: "Projects",
  props: {},
  components: {
    Hooper,
    Slide
  },
  data() {
    return {
      hooperSettings: {
        itemsToShow: 3,
        centerMode: true,
        infiniteScroll: false,
        wheelControl: false,
        breakpoints: {
          400: {
            centerMode: true,
            itemsToShow: 1
          },
          800: {
            centerMode: false,
            itemsToShow: 2
          },
          1000: {
            itemsToShow: 3,
            pagination: "fraction"
          }
        }
      }
    };
  }
};
</script>

<style scoped lang="stylus">
.projects
    padding 140px 0 0
.swiper-wrapper
    margin-bottom: 60px!important;
.block-wrapper
    display flex
    flex-direction column
    max-width 350px
.block-wrapper > img
    height auto
    background-color blue
    border-radius 6px 6px 0 0
    background-size: cover;
    max-width: 360px;
.block-info-content
    padding 40px
    display flex
    flex-direction column
    text-align left
    background-color #fff
    color #000
    border-radius 0 0 6px 6px
.title-project
    font-size 25px
    margin-bottom 10px
    font-weight 600
.info-about-project
    font-weight 400
    margin-bottom 20px
.gitHub-link
    padding: 10px 25px;
    max-width: 200px;
    border: 2px solid transparent;
    border-radius: 10px;
    border-image-source: linear-gradient(to right, #27a6e3 0%,#6200ab 100%)
    border-image-slice: 4;
.gitHub-link
    display flex
    flex-direction row
    align-items center
    text-decoration none
    text-align center
    justify-content center
.gitHub-logo
    max-width 35px
    margin-right 15px
.github
    color #000
    font-size 25px
    font-weight 500
    margin 0
.hooper
    height auto
    outline-width 0
@media only screen and (max-width: 1024px)
  .block-wrapper
    margin-right: 30px;
    max-width: 330px;
  .hooper-slide
    width 330px!important
@media only screen and (max-width: 600px)
  .block-wrapper
    max-width: 330px;
</style>
