<template>
  <div class="wrapper">
    <div class="title-section">
      <div class="left-column">
        <p>Hello, my name is</p>
        <p class="name">Georgi Nikolov</p>
        <p>I am a Front end Developer</p>
        <button class="btn-head btn-about">About</button>
        <button class="btn-head btn-contact">Contact</button>
      </div>
      <div class="right-column"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TitleSection"
};
</script>

<style scoped lang="stylus">
.title-section
  display flex
  flex-direction row
.left-column
  width 50%
.left-column
  width 50%
  text-align: left;
  padding: 140px 0;
p
  font-size 30px
  font-weight: 400;
  line-height: 80px;
.name
  font-size 70px
  font-weight 600
.btn-head
  padding 22px 45px
  font-size 30px
  font-weight 600
  border-radius: 7px;
  margin-top 20px
.btn-about
  margin-right: 60px;
  border 1px solid #fff
.btn-contact
  background-color: transparent;
  border 1px solid #fff
  color #fff
</style>
