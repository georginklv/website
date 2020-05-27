<template>
  <div class="wrapper" id="experience">
    <div class="experience">
      <div class="left-colum-experience">
        <p class="small-title">Qualification</p>
        <h2 class="heading heading-education">My Education</h2>
        <swiper class="swiper" :options="swiperOption">
          <swiper-slide>
            <div class="positions">
              <p class="position-small-title">Masters</p>
              <h2 class="heading-position">Economical University</h2>
              <p class="date">09.2017 - Present</p>
              <p class="paragraph">
                Master in "Business information systems"<br />
                - Creating Web Apps with HTML5, CSS3, JavaScript, jQuery<br />
                - Graphic Design with Adobe product
              </p>
            </div>

            <div class="positions">
              <p class="position-small-title">Bachelor</p>
              <h2 class="heading-position">Economical University</h2>
              <p class="date">09.2017 - 05.2017</p>
              <p class="paragraph">
                Bachelor in "Business information systems"<br />
                - Develop Economical skills also skill at accounting, marketing
                and law <br />- Develop programming skills at C#, Java and
                JavaScript<br />
                - Web Design<br />
                - Graphic Design
              </p>
            </div>
          </swiper-slide>

          <swiper-slide>
            <div class="positions">
              <h2 class="heading-position">Udemy</h2>
              <p class="paragraph">
                - Building Responsive Websites with HTML5 and CSS3<br />
                - Advanced CSS and Sass<br />
                - JavaScript
              </p>
            </div>

            <div class="positions">
              <h2 class="heading-position">Device Expert Academy</h2>
              <p class="paragraph">
                - JavaScript and jQuery<br />
                - Graphic Design <br />
                - Web Design
              </p>
            </div>
          </swiper-slide>

          <div class="swiper-button-prev" slot="button-prev"></div>
          <div class="swiper-button-next" slot="button-next"></div>
        </swiper>
      </div>
      <div class="right-colum-experience">
        <p class="small-title">All Companies</p>
        <h2 class="heading heading-education">My Experience</h2>

        <swiper class="swiper" :options="swiperOption">
          <swiper-slide>
            <div class="positions">
              <p class="position-small-title">Dopamine</p>
              <h2 class="heading-position">Front End Developer</h2>
              <p class="date">9.01.19 - Present</p>
              <p class="paragraph">
                Developing software applications<br />
                - Working on a team projects<br />
                - Making configurations for products via JavaScripts, working
                with frameworks (Vue)<br />
                - Creating layouts for jackpots via HTML5 and CSS3 (Stylus,
                sass)
              </p>
            </div>
            <div class="positions">
              <p class="position-small-title">Square Consultancy</p>
              <h2 class="heading-position">
                Web Developer and Graphic designer
              </h2>
              <p class="date">18.04.18 - 8.1.19</p>
              <p class="paragraph">
                - Daily maintenance three sites : www.betsat.com ,
                www.superbetin.com , www.betpot.com and their affiliates.<br />
                - Design and develop landing pages, promotion pages and also
                optimize them. Daily work with CMS systems.<br />
                - Design banners from promotions, sport events, GIFs and other
                graphic objects.<br />
                - Taking care of UX, UI of the site and helping for SEO
              </p>
            </div>
          </swiper-slide>

          <swiper-slide>
            <div class="positions">
              <p class="position-small-title">Playground</p>
              <h2 class="heading-position">Customer service</h2>
              <p class="date">1.04.17 - 4.2.18</p>
              <p class="paragraph">
                - Maintenance of hardware - Customer suport
              </p>
            </div>
            <div class="positions">
              <p class="position-small-title">TaxBack</p>
              <h2 class="heading-position">
                Expert maketing
              </h2>
              <p class="date">18.04.18 - 8.1.19</p>
              <p class="paragraph">
                - Made reports from which i made mass emails. The emails were
                made as pages with HTML5 and CSS3. Also take care of part of the
                SEO, data analysis and date update.
              </p>
            </div>
          </swiper-slide>

          <swiper-slide>
            <div class="positions">
              <p class="position-small-title">
                Hapmton Jitney (New York City, USA)
              </p>
              <h2 class="heading-position">Bus attendant</h2>
              <p class="date">1.6.16 - 1.10.16</p>
              <p class="paragraph">
                - Face to face customer service
              </p>
            </div>
            <div class="positions">
              <p class="position-small-title">
                McKinley Chalet Resort (Alaska , USA)
              </p>
              <h2 class="heading-position">Busser</h2>
              <p class="date">1.6.15 - 1.10.15</p>
              <p class="paragraph">
                - Customer service
              </p>
            </div>
          </swiper-slide>

          <div class="swiper-button-prev" slot="button-prev"></div>
          <div class="swiper-button-next" slot="button-next"></div>
        </swiper>
      </div>
    </div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
export default {
  name: "Experience",
  props: {},
  components: {
    Swiper,
    SwiperSlide
  },
  data() {
    return {
      swiperOption: {
        slidesPerView: "auto",
        centeredSlides: true,
        spaceBetween: 30,
        pagination: {
          el: ".swiper-pagination",
          clickable: true
        },
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev"
        }
      }
    };
  }
};
</script>

<style scoped lang="stylus">
.experience
  display: flex;
  flex-direction: row;
.left-colum-experience
  width 50%
  text-align left
.right-colum-experience
  width 50%
  text-align left
.positions
  border-left: 5px solid transparent;
  padding: .5rem;
  border-radius: 5px;
  border-image-source: linear-gradient(to bottom, #27a6e3 0%,#6200ab 100%)
  border-image-slice: 4;
  padding-left: 40px;
  margin-left: 40px;
  position: relative;
  &:before
    content: '';
    height: 15px;
    width: 15px;
    position: absolute;
    top: 0;
    left: -11px;
    border: 1px solid transparent;
    border-radius: 30px;
    background: #f167ad;
.small-title
  color: #27a5e2;
.heading
  font-size: 40px;
  line-height: 80px;
.position-small-title
  font-weight: 300;
  font-size: 15px;
.heading-position
  font-size: 25px;
  line-height: 40px;
.date
  color: #27a5e2;
  font-weight: 300;
  font-size: 15px;
  margin-bottom 10px
.paragraph
  margin-bottom: 20px;
.swiper-button-prev
  right: 10%;
  top: 10%;
  left: unset;
.swiper-button-next
  top: 10%;
@media only screen and (max-width: 1024px)
  .experience
    flex-direction column
  .wrapper
    max-width: 770px
  .right-colum-experience
    width 100%
  .left-colum-experience
    width 100%
    margin-bottom 40px
  .swiper-button-prev
    top 4%
    right: 13%;
  .swiper-button-next
    top 4%
    right: 0px;
@media only screen and (max-width: 600px)
   .wrapper
     max-width: 400px;
@media only screen and (max-width: 450px)
  .wrapper
     max-width: 270px
  .swiper-slide
      margin-top: 80px!important
  .positions
      margin-left: 10px;
      &:before
        left: -10px;
</style>
