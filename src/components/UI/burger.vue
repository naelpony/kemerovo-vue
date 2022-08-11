<template>
  <Slide right>
    <ul class="menu__list">
      <li id="home" href="#">
        <div class="menu__link" @click="dropMenu">О Кемерово</div>
        <ul class="sabmenu__list">
          <li>
            <a href="" class="sabmenu__link">Обращение главы города Кемерово</a>
          </li>
          <li>
            <a href="" class="sabmenu__link"
              >Стратегия социально-экономического развития города</a
            >
          </li>
        </ul>
      </li>
      <li id="home" href="#">
        <div class="menu__link" @click="dropMenu">Малому бизнесу</div>
        <ul class="sabmenu__list">
          <li>
            <a href="" class="sabmenu__link">Обращение главы города Кемерово</a>
          </li>
          <li>
            <a href="" class="sabmenu__link"
              >Стратегия социально-экономического развития города</a
            >
          </li>
        </ul>
      </li>
      <li id="home" href="#">
        <div class="menu__link" @click="dropMenu">Инвестору</div>
        <ul class="sabmenu__list">
          <li>
            <a href="" class="sabmenu__link">Обращение главы города Кемерово</a>
          </li>
          <li>
            <a href="" class="sabmenu__link"
              >Стратегия социально-экономического развития города</a
            >
          </li>
        </ul>
      </li>
      <li id="home" href="#">
        <div class="menu__link" @click="dropMenu">Меры поддержки</div>
        <ul class="sabmenu__list">
          <li>
            <a href="" class="sabmenu__link">Обращение главы города Кемерово</a>
          </li>
          <li>
            <a href="" class="sabmenu__link"
              >Стратегия социально-экономического развития города</a
            >
          </li>
        </ul>
      </li>
      <li id="home" href="#">
        <div class="menu__link" @click="dropMenu">
          Инвестиционная деятельность
        </div>
        <ul class="sabmenu__list">
          <li>
            <a href="" class="sabmenu__link">Обращение главы города Кемерово</a>
          </li>
          <li>
            <a href="" class="sabmenu__link"
              >Стратегия социально-экономического развития города</a
            >
          </li>
        </ul>
      </li>
      <li id="home" href="#">
        <div class="menu__link" @click="dropMenu">ОРВ</div>
      </li>
      <li id="home" href="#">
        <div class="menu__link" @click="dropMenu">Обратная связь</div>
      </li>
    </ul>
  </Slide>
</template>
<script>
import { Slide } from "vue3-burger-menu";
let drop;
const dropMenu = () => {
  drop = document.querySelectorAll(".menu__link");
  if (drop.length > 0) {
    for (let i = 0; i < drop.length; i++) {
      let dropA = drop[i];
      dropA.addEventListener("click", function (e) {
        dropA.parentElement.classList.toggle("_activ");
      });
    }
  }
};
export default {
  components: {
    Slide,
  },
  data() {
    return {
      dropMenu,
    };
  },
};
</script>
<style lang="sass" scoped>
a
	text-decoration: none
li
	position: relative
	list-style: none
.menu__list
	display: flex
	flex-direction: column
.menu__list>li
	margin: 10px 0 0 0
.menu__list>li._activ .sabmenu__list
	display: block
.menu__link
	padding: 0
	font-weight: 300
	font-size: 20px
	line-height: 24px
	letter-spacing: 0.02em
	color: #484848
.sabmenu__list
	display: none
	position: relative
	padding: 10px 0 0 0
	width: 100%
	border-radius: 0px 0px 2px 2px
.sabmenu__list>li

	background: #FFFFFF
	text-align: start

	padding: 9px 7px
.sabmenu__list>li:hover
	background: #B8B3B3
.sabmenu__link
	font-style: normal
	font-weight: 400
	font-size: 12px
	line-height: 14px
	letter-spacing: 0.02em

	color: #484848
</style>