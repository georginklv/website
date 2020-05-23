<template>
  <div class="wrapper">
    <div class="nav-bar">
      <div class="nav-items">
        <a href="#" class="btn btn-nav">Home</a>
        <a href="#" class="btn btn-nav">About</a>
        <a href="#" class="btn btn-nav">Expirience</a>
        <a href="#" class="btn btn-nav">Projects</a>
        <a href="#" class="btn btn-nav">Contact</a>
      </div>
      <a href="#" class="btn logo">georginklv</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  props: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
.nav-bar
  display flex
  flex-direction row
  justify-content space-between
  height 100px
  align-items center
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
.btn-nav:hover
  color #61048d
</style>
