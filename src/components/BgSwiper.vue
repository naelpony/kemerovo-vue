<template>
  <swiper
    class="swiper"
    :modules="modules"
    :effect="'fade'"
    :allow-touch-move="false"
    :pagination="{ clickable: false, renderBullet: bulletRenderer }"
    :autoplay="{
      delay: 50000,
      disableOnInteraction: false,
    }"
  >
    <swiper-slide class="slide"
      ><img src="../assets/img/slidone.png" alt=""
    /></swiper-slide>
    <swiper-slide class="slide"
      ><img src="../assets/img/slidtwo.png" alt=""
    /></swiper-slide>
    <swiper-slide class="slide"
      ><img src="../assets/img/slidthree.png" alt=""
    /></swiper-slide>
  </swiper>
</template>

<script >
import { defineComponent } from "vue";
import { Pagination, EffectFade, Autoplay } from "swiper";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css/effect-fade";
import "swiper/css";
import "swiper/css/pagination";

export default defineComponent({
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const bulletRenderer = (index, className) => {
      const _className = `${className} swiper-pagination-bullet-custom`;
      return `<span class="${_className}">
								<p>
									0${index + 1}
								</p>
							</span>
              
              `;
    };

    return {
      bulletRenderer,
      modules: [Pagination, EffectFade, Autoplay],
    };
  },
});
</script>

<style lang="sass" scoped>
.swiper
  position: absolute
  height: 1000px
  z-index: -2
  top: 0
  bottom: 0
  left: 0
  right: 0
  opacity: 1
  overflow: hidden
  ::v-deep(.swiper-pagination-bullet-custom)

    margin: 0 0 340px 10px
    width: 50px
    height: 6px
    box-sizing: border-bo
    background: #F4F4F4
    border-radius: 1px
    opacity: 1

    & p
      font-style: normal
      font-weight: 800
      font-size: 14px
      line-height: 17px
      letter-spacing: 0.02em
      margin: 9px 0 0 0
      color: #F4F4F4

    &.swiper-pagination-bullet-active
      background: #B5464A
      & p
        font-style: normal
        font-weight: 800
        font-size: 20px
        line-height: 24px
        letter-spacing: 0.02em
        margin: 3px 0 0 0
        color: #B5464A
img
  width: 100%
  height: 100%

  object-fit: cover
  background: radial-gradient(64.04% 64.04% at 50% 35.96%, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.4) 32.78%, rgba(0, 0, 0, 0.5) 100%)

.slide
  position: relative
  display: inline-block
  &::after
    content: ""
    display: block
    width: 100%
    height: 100%
    position: absolute
    top: 0
    left: 0
    background: transparent
    background-image: radial-gradient(64.04% 64.04% at 50% 35.96%, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.4) 32.78%, rgba(0, 0, 0, 0.5) 100%)
    opacity: 0.7

@media screen and (max-width: 1410px )
  .swiper
    height: 700px
    ::v-deep(.swiper-pagination-bullet-custom)
      margin: 0 0 190px 10px
      width: 40px
      height: 5px
      &:hover

      & p
        font-size: 12px
        line-height: 17px

      &.swiper-pagination-bullet-active
        background: #B5464A
        & p
          font-size: 16px
          line-height: 24px
@media screen and (max-width: 810px )
  .swiper
    height: 550px
@media screen and (max-width: 425px )
  .swiper
    ::v-deep(.swiper-pagination-bullet-custom)
      margin: 0 0 100px 10px
      width: 40px
      height: 5px
</style>