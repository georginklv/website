<template>
  <div class="wrapper wrapper-nav-bar">
    <div class="nav-bar" @scroll="handleSCroll">
      <b-navbar toggleable type="dark" variant="dark" class="mobileNav">
        <b-navbar-brand href="#" class="logo logo-mobile"
          >georginklv</b-navbar-brand
        >

        <b-navbar-toggle target="navbar-toggle-collapse">
          <template v-slot:default="{ expanded }">
            <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
            <b-icon v-else icon="chevron-bar-down"></b-icon>
          </template>
        </b-navbar-toggle>

        <b-collapse id="navbar-toggle-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item href="#">Home</b-nav-item>
            <b-nav-item href="#about">About</b-nav-item>
            <b-nav-item href="#experience">Experience</b-nav-item>
            <b-nav-item href="#projects">Projects</b-nav-item>
            <b-nav-item href="#contact">Contact</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
      <div class="nav-items">
        <ul class="main-nav" id="js-manu">
          <li>
            <a href="#" class="btn btn-nav">Home</a>
          </li>
          <li>
            <a href="#about" class="btn btn-nav">About</a>
          </li>
          <li>
            <a href="#experience" class="btn btn-nav">Experience</a>
          </li>
          <li>
            <a href="#projects" class="btn btn-nav">Projects</a>
          </li>
          <li>
            <a href="#contact" class="btn btn-nav">Contact</a>
          </li>
        </ul>
      </div>
      <a href="#" class="btn logo">georginklv</a>
    </div>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
export default {
  name: "NavBar",
  props: {},
  methods: {
    // eslint-disable-next-line no-unused-vars
    handleSCroll(event) {
      let header = document.querySelector(".wrapper-nav-bar");
      if (window.scrollY > 20 && !header.className.includes("anime")) {
        header.classList.add("anime");
      } else if (window.scrollY < 20) {
        header.classList.remove("anime");
      }
    }
  },
  created() {
    window.addEventListener("scroll", this.handleSCroll);
  },
  destroyed() {
    window.removeEventListener("scroll", this.handleSCroll);
  }
};
</script>

<!-- /* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {...}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {...}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {...} -->
<style scoped lang="stylus">


  .mobileNav
    display none
  .wrapper-nav-bar
    position fixed
    top: 0;
    right: 0;
    left: 0;
    max-width none
    z-index: 1000;
    transition: linear 0.2s;
  .anime
    height auto
    background-color #000c
    backdrop-filter blur(20px)
  .main-nav
    list-style-type none
    display flex
    flex-direction row
    align-items center
  .nav-bar
    display flex
    flex-direction row
    justify-content space-between
    align-items center
    max-width: 1400px;
    margin: 0 auto;
  ul
    margin 0
  li
    margin-right 30px
  .btn
    text-decoration none
    color #fff
    margin-right 30px
    font-weight 600
    font-size 25px
    padding 0
  .btn:last-of-type
    margin-right 0
  .logo
    display block
    font-size 40px
    font-weight 800
    z-index 1
    text-shadow 7px 8px 11px #000
    padding-right: 30px;
  .btn-nav
    transition: linear 0.2s;
    padding 0
    &:hover
        color #61048d


/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (max-width: 1024px)
    .main-nav
      display: none;
    .mobileNav
      display flex
      background-color: #000!important;
      padding: 10px 40px;
      width: 100%;
    .logo
        display: none;
    .logo-mobile
      display block
      font-size: 25px;
      font-weight: 500;
    .nav-bar
      height: auto;
</style>
