<template>
  <div class="wrapper">
    <div class="title-section">
      <div class="left-column">
        <p>Hello, my name is</p>
        <p class="name">Georgi Nikolov</p>
        <p>I am a Front end Developer</p>
        <a href="#about" class="btn-head btn-about">About</a>
        <a href="#contact" class="btn-head btn-contact">Contact</a>
      </div>
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
    color #000
    text-decoration none
  .btn-about
    cursor pointer
    margin-right: 60px;
    border 1px solid #fff
    transition linear 0.2s
    background-color #fff
    &:hover
      border 1px solid #61048d
      color #61048d
      background-color #000
      text-decoration none
  .btn-contact
    cursor pointer
    background-color: transparent;
    border 1px solid #fff
    color #fff
    transition linear 0.2s
    &:hover
      border 1px solid #61048d
      color #61048d
      text-decoration none


@media only screen and (max-width: 1024px)
    .title-section
      justify-content: center;
      margin-top 80px
    .left-column
      width: 60%;
      margin: 0 auto;
      padding 30px 40px
      background #000
      border-radius 20px
      background: #000000c7;
      backdrop-filter: blur(20px);
    .btn-about
      margin-right: 20px;
    .name
      font-size: 55px;
    p
      font-size: 25px;
    .btn-about
      background-color #fff
@media only screen and (max-width: 768px)
  .left-column
      width: 100%;
      border-radius 0px
  .title-section
    justify-content: center;
    margin-top 40px
  .name
    font-size: 65px;

@media only screen and (max-width: 600px)
  .left-column
    padding 40px
  .name
    font-size 60px
  p
    font-size 25px
  .btn-head
    padding: 12px 35px;
    font-size: 20px;
    margin-top: 20px;
  .btn-about
    margin-right: 30px;
@media only screen and (max-width: 450px)
  .name
    font-size 40px
  .btn-about
    margin-right: 10px;
  p
    font-size: 17px;
    line-height: 50px;
</style>
