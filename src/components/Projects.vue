<template>
  <div class="wrapper">
    <div class="projects">
      <hooper :itemsToShow="3" :centerMode="true">
        <slide :index="0">
          <div class="block-wrapper">
            <div class="img"></div>
            <!--img src="" alt="" class="block-"-->
            <div class="block-info-content">
              <p class="title-project">Project</p>
              <p class="info-about-project">allalalvkajvlkajsklvjaklsv</p>
              <a href="" class="gitHub-link">
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
            <div class="img"></div>
            <!--img src="" alt="" class="block-"-->
            <div class="block-info-content">
              <p class="title-project">Project</p>
              <p class="info-about-project">allalalvkajvlkajsklvjaklsv</p>
              <a href="" class="gitHub-link">
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
            <div class="img"></div>
            <!--img src="" alt="" class="block-"-->
            <div class="block-info-content">
              <p class="title-project">Project</p>
              <p class="info-about-project">allalalvkajvlkajsklvjaklsv</p>
              <a href="" class="gitHub-link">
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
  data() {}
};
</script>

<style scoped lang="stylus">
.projects
    padding 140px 0
.swiper-wrapper
    margin-bottom: 60px!important;
.block-wrapper
    display flex
    flex-direction column
    max-width 350px
.img
    height 210px
    background-color blue
    border-radius 6px 6px 0 0
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
.hooper
    height auto
</style>
