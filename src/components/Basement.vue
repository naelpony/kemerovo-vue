<template>
  <div class="container">
    <div class="wrapper">
      <div class="foot-menu">
        <div class="pcc">
          <logo />
        </div>
        <div class="phonee">
          <div class="logo">
            <img src="../assets/img/logo.png" alt="" />
            <div class="title">
              <h2>Инвестиционный портал</h2>
              <h1>города Кемерово</h1>
            </div>
          </div>
          <div class="language">
            <select>
              <option>CH</option>
              <option>ENG</option>
              <option selected>RU</option>
            </select>
          </div>
        </div>
        <ul class="menu__list">
          <li class="menu__item" v-for="items in arr" :key="items.id">
            <a href="">{{ items.name }}</a>
          </li>
        </ul>
      </div>
      <p>Для связи по инвест проектам prom3@kemerovo.ru</p>
    </div>
  </div>
</template>
<script>
import Logo from "./UI/logo.vue";

const arr = [
  { id: 0, name: "О Кемерово" },
  { id: 1, name: "Инвестиционная деятельность" },
  { id: 2, name: "Малому бизнесу" },
  { id: 3, name: "Обратная связь" },
  { id: 4, name: "ОРВ" },
];

export default {
  components: { Logo },
  data() {
    return {
      arr,
    };
  },
};
</script>
<style lang="sass" scoped>
.phonee
	display: none
.pcc
	max-width: 370px
	width: 100%
.container
	background: #212121
	margin: 21px 0 0 0
.wrapper
	max-width: 1410px
	margin: 0 auto
	display: flex
	flex-direction: column
	padding: 32px 0 0 0
.foot-menu
	display: flex
	align-items: flex-end
.menu__list
	margin: 0 0 0 100px
	padding: 0
	width: 100%
	display: flex
	justify-content: space-between
	align-items: flex-start
.menu__item
	max-width: 194px
	padding: 0 50px 0 0
	&:last-child
		padding: 0

a
	font-style: normal
	width: 100%
	font-weight: 500
	font-size: 20px
	line-height: 24px
	color: #FFFFFF
	letter-spacing: 0.02em
	&:hover
		color: green
p
	align-self: flex-end
	font-style: normal
	font-weight: 400
	font-size: 14px
	line-height: 17px
	margin: 62px 0 50px 0
	text-align: right
	letter-spacing: 0.02em

	color: #FFFFFF

@media screen and (max-width: 1410px )
	.wrapper
		margin: 0 15px
	.menu__list
		margin: 0 0 0 50px
	.menu__item
		max-width: 150px
		padding: 0 30px 0 0
		&:last-child
			padding: 0

	a
		width: 100%
		font-size: 16px
		line-height: 20px
	p
		font-size: 12px
		line-height: 16px
		margin: 42px 0 35px 0
@media screen and (max-width: 1110px)
	.wrapper
		margin: 0 15px
	.menu__list
		margin: 0 0 0 25px
	.menu__item
		max-width: 150px
		padding: 0 10px 0 0
		&:last-child
			padding: 0

	a
		width: 100%
		font-size: 12px
		line-height: 20px
	p
		font-size: 12px
		line-height: 10px
		margin: 42px 0 35px 0
@media screen and (max-width: 810px )
	.phonee
		display: flex
		align-items: center
		width: 100%
	.pcc
		display: none
	.menu__list
		flex-direction: column
		flex-wrap: wrap
	.logo
		display: flex
		align-items: center
		max-width: 225px
		width: 100%
		padding: 0 10px 0 0
		& h2
			font-style: normal
			font-weight: 300
			font-size: 10px
			line-height: 17px
			color: #FFFFFF
			margin: 0
		& h1
			font-style: normal
			font-weight: 800
			font-size: 14px
			line-height: 24px
			letter-spacing: 0.02em
			color: #E7E7E7
			margin: 0
		& img
			width: 30%
			margin: 0 10px 0 0
	.language
		padding: 0 10px 0 0
		& select
			background: none
			border: none
			border-bottom: 1px solid white
			font-style: normal
			font-weight: 300
			font-size: 14px
			line-height: 150%

			text-transform: uppercase

			color: rgba(255, 255, 255, 0.8)
			color: white
			padding: 0 0 4px 0
			&:active
				outline: none
			&:focus
				outline: none
		& option
			background: #000
			border: #000
			font-style: normal
			font-weight: 300
			font-size: 14px
			line-height: 150%

			text-transform: uppercase

			color: rgba(255, 255, 255, 0.8)
</style>