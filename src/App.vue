<template>
  <div id="app">
    <img src="./assets/head-img.png" alt="" class="head-img" />

    <NavBar />
    <TitleSection />
    <About />
    <Experience />
    <Projects />
    <Footer />
    <img src="./assets/footer.png" alt="" class="footer-img" />
  </div>
</template>
<script>
import NavBar from "./components/NavBar.vue";
import TitleSection from "./components/TitleSection.vue";
import About from "./components/About.vue";
import Experience from "./components/Experience.vue";
import Projects from "./components/Projects.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    NavBar,
    TitleSection,
    About,
    Experience,
    Projects,
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
  overflow-x: hidden;

.wrapper
  width 100%
  max-width 1400px
  margin 0 auto
  position relative
  z-index 10
.head-img
  position absolute
  right 0
.footer-img
  position: absolute;
  left: 0;
  bottom: 0;
body::-webkit-scrollbar
  width: 1em;
body::-webkit-scrollbar-track
  box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
body::-webkit-scrollbar-thumb
  background: linear-gradient(to bottom, #27a6e3 0%,#6200ab 100%);
  outline: 1px solid slategrey;
.nav-wrapper
  display flex
  flex-direction row

#navigation-icon
  padding 10px 10px 20px
  margin-right 10px
  cursor pointer
i
  font-size 2rem
  width 100px
  height 100px
  background #fff
</style>
