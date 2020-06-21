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
              <h2 class="heading-position">Economic University</h2>
              <p class="date">01.09.2017 - Present</p>
              <ul class="paragraph">
                <p>Master in "Business information systems"</p>
                <li>Creating Web Apps with HTML5, CSS3, JavaScript, jQuery</li>
                <li>Graphic Design with Adobe product</li>
              </ul>
            </div>

            <div class="positions">
              <p class="position-small-title">Bachelor</p>
              <h2 class="heading-position">EconomicUniversity</h2>
              <p class="date">01.09.2013 - 05.2017</p>
              <ul class="paragraph">
                <p>Bachelor in "Business information systems</p>
                <li>
                  Develop Economic skills also skill at accounting, marketing
                  and law
                </li>
                <li>Develop programming skills at C#, Java andJavaScript</li>
                <li>Web Design</li>
                <li>Graphic Design</li>
              </ul>
            </div>
          </swiper-slide>

          <swiper-slide>
            <div class="positions">
              <h2 class="heading-position">Udemy</h2>
              <ul class="paragraph">
                <li>Building Responsive Websites with HTML5 and CSS3</li>
                <li>Advanced CSS and Sass</li>
                <li>JavaScript</li>
              </ul>
            </div>

            <div class="positions">
              <h2 class="heading-position">Device Expert Academy</h2>
              <ul class="paragraph">
                <li>JavaScript and jQuery</li>
                <li>Graphic Design</li>
                <li>Web Design</li>
              </ul>
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
              <p class="date">09.01.19 - Present</p>
              <ul class="paragraph">
                <li>Developing software applications</li>
                <li>Working on a team projects</li>
                <li>
                  Making configurations for products via JavaScripts, working
                  with frameworks (Vue)
                </li>
                <li>
                  Creating layouts for jackpots via HTML5 and CSS3 (Stylus,
                  sass)
                </li>
              </ul>
            </div>
            <div class="positions">
              <p class="position-small-title">Square Consultancy</p>
              <h2 class="heading-position">
                Web Developer and Graphic designer
              </h2>
              <p class="date">18.04.18 - 08.01.19</p>
              <ul class="paragraph">
                <li>
                  Daily maintenance three sites : www.betsat.com ,
                  www.superbetin.com , www.betpot.com and their affiliates.
                </li>
                <li>
                  Designing and develop landing pages, promotion pages and also
                  optimize them. Daily work with CMS systems.
                </li>
                <li>
                  Designing banners from promotions, sport events, GIFs and
                  other graphic objects.
                </li>
                <li>Taking care of UX, UI of the site and helping for SEO</li>
              </ul>
            </div>
          </swiper-slide>

          <swiper-slide>
            <div class="positions">
              <p class="position-small-title">Playground</p>
              <h2 class="heading-position">Customer service</h2>
              <p class="date">01.04.17 - 04.02.18</p>
              <ul class="paragraph">
                <li>Maintenance of hardware - Customer suport</li>
              </ul>
            </div>
            <div class="positions">
              <p class="position-small-title">TaxBack</p>
              <h2 class="heading-position">
                Marketing expert
              </h2>
              <p class="date">18.04.18 - 08.01.19</p>
              <ul class="paragraph">
                <li>
                  Made reports from which i made mass emails.
                </li>
                <li>
                  Emails were made as pages with HTML5 and CSS3.
                </li>
                <li>
                  Take care of part of the SEO, data analysis and date update.
                </li>
              </ul>
            </div>
          </swiper-slide>

          <swiper-slide>
            <div class="positions">
              <p class="position-small-title">
                Hapmton Jitney (New York City, USA)
              </p>
              <h2 class="heading-position">Bus attendant</h2>
              <p class="date">01.6.16 - 01.10.16</p>
              <ul class="paragraph">
                <li>Face to face customer service</li>
              </ul>
            </div>
            <div class="positions">
              <ul class="position-small-title">
                <li>McKinley Chalet Resort (Alaska , USA)</li>
              </ul>
              <h2 class="heading-position">Busser</h2>
              <p class="date">01.06.15 - 01.10.15</p>
              <ul class="paragraph">
                <li>Customer service</li>
              </ul>
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
  border-right: 0px;
  border-top: 0px;
  &:before
    content: '';
    height: 15px;
    width: 15px;
    position: absolute;
    top: 0;
    left: -10px;
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
    right: 20px;
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
