<template>
  <div class="wrapper">
    <div class="about">
      <div class="left-column"></div>
      <div class="right-column">
        <h2 class="title title-about">About</h2>
        <div class="line"></div>
        <p class="who">Who am I</p>
        <p class="paragraph">
          Truly motivated, communicative person, who wants to learn something
          new everyday and develop himself . Facing business related issues and
          contribute towards the success of the company. Hard work and time
          management are crucial part of day-to-day work.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  props: {}
};
</script>

<style scoped lang="stylus">
.about
    padding 140px 0
    display flex
    flex-direction row
    text-align left
h2
    font-size 50px
.line
    margin 20px 0
    width 200px
    height 3px
    background: linear-gradient(to right, #27a6e3 0%,#6200ab 100%);
.left-column
    width 50%
.right-column
    width 50%
.who
    font-size 40px
    margin-bottom 40px
.paragraph
    font-size: 20px;
    font-weight: 400;
    color: #ffffffb3;
    line-height: 30px;
</style>
