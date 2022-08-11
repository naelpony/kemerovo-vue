<template>
  <div class="container">
    <div class="wrapper">
      <swiper
        class="swiper"
        :modules="modules"
        @swiper="setVSwiperRef"
        :slides-per-view="pageWidth > 810 ? 3 : 1"
        @slide-change="updateVSwiperIndex"
      >
        <swiper-slide class="slide" v-for="items in arr" :key="items.id"
          ><img :src="items.img" alt=""
        /></swiper-slide>
      </swiper>
      <button class="nav-button-prev" @click="prevVSwiperSlide"></button>
      <button class="nav-button-next" @click="nextVSwiperSlide"></button>
    </div>
  </div>
</template>
<script>
import { defineComponent, ref } from "vue";
import { Pagination, Navigation, Grid, Mousewheel } from "swiper";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";

import pic1 from "../assets/img/slide1.png";
import pic2 from "../assets/img/slide2.png";
import pic3 from "../assets/img/slide3.png";

const arr = [
  { id: 0, img: pic1 },
  { id: 1, img: pic2 },
  { id: 2, img: pic3 },
  { id: 3, img: pic1 },
  { id: 4, img: pic2 },
  { id: 5, img: pic3 },
  { id: 6, img: pic1 },
  { id: 7, img: pic2 },
  { id: 8, img: pic3 },
  { id: 9, img: pic1 },
  { id: 10, img: pic2 },
  { id: 11, img: pic3 },
  { id: 12, img: pic1 },
  { id: 13, img: pic2 },
  { id: 14, img: pic3 },
];

export default defineComponent({
  name: "swiper-example-default",
  title: "Default",
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    let vSwiperRef = null;
    const setVSwiperRef = (swiper) => {
      vSwiperRef = swiper;
    };
    const vSwiperIndex = ref();
    const updateVSwiperIndex = () => {
      vSwiperIndex.value = vSwiperRef?.activeIndex;
    };
    const prevVSwiperSlide = () => vSwiperRef?.slidePrev();
    const nextVSwiperSlide = () => vSwiperRef?.slideNext();

    const pageWidth = document.documentElement.scrollWidth;
    return {
      modules: [Navigation],
      arr,
      pageWidth,

      setVSwiperRef,
      updateVSwiperIndex,
      prevVSwiperSlide,
      nextVSwiperSlide,
    };
  },
});
</script>
<style lang="sass" scoped>
.container
  background: linear-gradient(0deg, rgba(68, 35, 35, 0.4), rgba(68, 35, 35, 0.4)), url( ../assets/img/bgslider.png)
  margin: 62px 0 0 0
.wrapper
  max-width: 1410px
  margin: 0 auto
  position: relative
  padding: 130px 0
.swiper
  max-width: 1170px
  position: relative
  overflow: hidden
.nav-button-prev
  position: absolute
  cursor: pointer
  top: 50%
  left: 0
  z-index: 9
  background: url(../assets/img/arrow.png) #D53A3F no-repeat center center
  border-radius: 50%
  border: none
  height: 45px
  width: 45px
  margin: 0 15px 0 0
  transform: rotate(180deg)

.nav-button-next
  position: absolute
  cursor: pointer
  top: 50%
  right: 0
  z-index: 9
  background: url(../assets/img/arrow.png) #D53A3F no-repeat center center
  border-radius: 50%
  border: none
  height: 45px
  width: 45px
  margin: 0 15px 0 0

@media screen and (max-width: 1410px )
  .container
    margin: 42px 0 0 0
  .wrapper
    margin: 0 15px
    padding: 100px 0
    overflow: hidden
  .swiper
    max-width: 860px
  .nav-button-prev
    position: absolute
    cursor: pointer
    top: 50%
    left: 0
    z-index: 9
    background: url(../assets/img/arrow.png) #D53A3F no-repeat center center
    border-radius: 50%
    border: none
    height: 35px
    width: 35px
    margin: 0 10px 0 0
    transform: rotate(180deg)

  .nav-button-next
    position: absolute
    cursor: pointer
    top: 50%
    right: 0
    z-index: 9
    background: url(../assets/img/arrow.png) #D53A3F no-repeat center center
    border-radius: 50%
    border: none
    height: 35px
    width: 35px
    margin: 0 10px 0 0
  img
    width: 270px
@media screen and (max-width: 1110px )
  .container
    margin: 42px 0 0 0
  .wrapper
    margin: 0 15px
    padding: 100px 0
    overflow: hidden
  .swiper
    max-width: 700px
  .nav-button-prev
    position: absolute
    cursor: pointer
    top: 50%
    left: 0
    z-index: 9
    background: url(../assets/img/arrow.png) #D53A3F no-repeat center center
    border-radius: 50%
    border: none
    height: 35px
    width: 35px
    margin: 0 10px 0 0
    transform: rotate(180deg)

  .nav-button-next
    position: absolute
    cursor: pointer
    top: 50%
    right: 0
    z-index: 9
    background: url(../assets/img/arrow.png) #D53A3F no-repeat center center
    border-radius: 50%
    border: none
    height: 35px
    width: 35px
    margin: 0 10px 0 0
  img
    width: 200px
@media screen and (max-width: 810px )
  .container
    margin: 42px 0 0 0
  .wrapper
    margin: 0 15px
    padding: 100px 0
    overflow: hidden
  .swiper
    max-width: 500px
    justify-content: center
    align-items: center
  .swiper-slide
    display: flex
    justify-content: center
  img
    width: 250px
</style>