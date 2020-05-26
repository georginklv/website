<template>
  <div class="wrapper wrapper-nav-bar">
    <div class="nav-bar" @scroll="handleSCroll">
      <div class="nav-items">
        <a href="#" class="btn btn-nav">Home</a>
        <a href="#about" class="btn btn-nav">About</a>
        <a href="#experience" class="btn btn-nav">Expirience</a>
        <a href="#projects" class="btn btn-nav">Projects</a>
        <a href="#contact" class="btn btn-nav">Contact</a>
      </div>
      <a href="#" class="btn logo">georginklv</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  props: {},
  methods: {
    // eslint-disable-next-line no-unused-vars
    handleSCroll(event) {
      let header = document.querySelector(".wrapper-nav-bar");
      if (window.scrollY > 100 && !header.className.includes("anime")) {
        header.classList.add("anime");
      } else if (window.scrollY < 100) {
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
.wrapper-nav-bar
  position fixed
  top: 0;
  right: 0;
  left: 0;
  max-width none
  z-index: 1000;
  transition: linear 0.2s;
.anime
  background-color #000c
  backdrop-filter blur(20px)
.nav-bar
  display flex
  flex-direction row
  justify-content space-between
  height 100px
  align-items center
  max-width: 1400px;
  margin: 0 auto;
.btn
  text-decoration none
  color #fff
  margin-right 30px
  font-weight 600
  font-size 25px
.btn:last-of-type
  margin-right 0
.logo
  font-size 40px
  font-weight 800
  z-index 1
  text-shadow 7px 8px 11px #000
.btn-nav
  transition: linear 0.2s;
  &:hover
      color #61048d
</style>
