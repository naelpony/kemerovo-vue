<template>
  

  <header class="header">
    <bg-swiper />
    <div class="head">  
      <div class="pc">
        <head-search />
        <head-menu />
      </div>
      <div class="phone">
        <div class="phone-c">
          <phone/>
          <burger/>
        </div>
      </div>
    </div>
    <div class="main">
      <icon />
    </div>
    <div class="card-phone">
      <card />
    </div>
  </header>
  <message />
  <news />
  <answer />
  <foot-slider />
  <div class="black">
    <input-search-black />
  </div>
  <basement />
</template>
<script>
import BgSwiper from "@/components/BgSwiper.vue";
import HeadMenu from "@/components/HeadMenu.vue";
import HeadSearch from "@/components/HeadSearch.vue";
import Icon from "./components/Icon.vue";
import Card from "./components/Card.vue";
import Message from "./components/Message.vue";
import News from "./components/News.vue";
import Answer from "./components/Answer.vue";
import FootSlider from "./components/FootSlider.vue";
import InputSearchBlack from "./components/UI/input-search-black.vue";
import Burger from "./components/UI/burger.vue";
import Basement from "./components/Basement.vue";
import Phone from "./components/Phone.vue";
export default {
  components: {
    BgSwiper,
    HeadSearch,
    HeadMenu,
    Icon,
    Card,
    Message,
    News,
    Answer,
    FootSlider,
    InputSearchBlack,
    Burger,
    Basement,
    Phone,
  },
};
</script>
