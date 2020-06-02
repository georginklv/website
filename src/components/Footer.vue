<template>
  <div class="footer">
    <div class="wrapper" id="contact">
      <div class="block-footer">
        <div class="inner-container">
          <h2 class="title">Contact me</h2>
          <div class="line"></div>
          <div class="footer-row">
            <img
              src="../assets/phone.png"
              alt=""
              class="footer-small-img phone"
            />
            <p>+359 878 67 48 25</p>
          </div>
          <div class="footer-row">
            <img
              src="../assets/mail.png"
              alt=""
              class="footer-small-img mail"
            />
            <a href="mailto: georginklv@abv.bg" target="_blank"
              >georginklv@abv.bg</a
            >
          </div>
          <div class="footer-row">
            <img
              src="../assets/linkedin.png"
              alt=""
              class="footer-small-img linkedin"
              target="_blank"
            />
            <a
              href="https://www.linkedin.com/in/georgi-nikolov-b43816139/"
              target="_blank"
              >Georgi Nikolov</a
            >
          </div>
          <div class="footer-row">
            <img
              src="../assets/github.png"
              alt=""
              class="footer-small-img github"
            />
            <a href="https://github.com/georginklv" target="_blank"
              >georginklv</a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  props: {}
};
</script>

<style scoped lang="stylus">
.footer
    position relative
    padding 140px 0
.wrapper
    position relative
.line
    margin 10px auto 40px
    width 200px
    height 3px
    background: linear-gradient(to right, #27a6e3 0%,#6200ab 100%);
.footer-img
    position absolute
    left 0
    bottom 0
.block-footer
    background #ffffff
    border-radius 15px
    z-index 1
    margin: 0 auto;
    max-width: 900px;
    color #000
    position: relative;
    padding: 80px 140px
.footer-row
    display flex
    flex-direction row
    margin-bottom 20px
    align-items: center;
.footer-small-img
    max-width 35px
    margin-right 150px
.title
    font-size 40px
p,a
    font-size: 30px;
    font-weight: 500;
    text-decoration: none;
    color: #000;
@media only screen and (max-width: 1024px)
  .block-footer
    padding: 20px 30px;
  .footer-small-img
    margin-right 25px
  a,
  p
    font-size 20px
</style>
