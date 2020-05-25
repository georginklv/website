<template>
  <div id="app">
    <img src="./assets/head-img.png" alt="" class="head-img" />
    <NavBar />
    <TitleSection />
    <About />
    <Experience />
    <Footer />
    <img src="./assets/footer.png" alt="" class="footer-img" />
  </div>
</template>
<script>
import NavBar from "./components/NavBar.vue";
import TitleSection from "./components/TitleSection.vue";
import About from "./components/About.vue";
import Experience from "./components/Experience.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    NavBar,
    TitleSection,
    About,
    Experience,
    Footer
  }
};
</script>

<style lang="stylus">
*
  margin 0
  padding 0
  box-sizing border-box
body
  background-color #000
  width: 100vw;
  overflow-x: hidden;
#app
  font-family Roboto, sans-serif
  text-align center
  color #fff
  max-width 1920px
  margin 0 auto
  position relative
.wrapper
  width 100%
  max-width 1400px
  margin 0 auto
  position relative
  z-index 10
.head-img
  position absolute
.footer-img
  position: absolute;
  left: 0;
  bottom: 0;
</style>
