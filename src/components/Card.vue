<template>
  <div class="container">
      <div class="card" v-for="items in arr" :key="items.id">
        <div class="head">
          <span class="arrow"></span>
          <h1>{{ items.title }}</h1>
        </div>
        <div class="show__text">
					<img :src="items.img" alt="">
          <div class="text">
            <h1>
              {{ items.text }}
            </h1>
            <p>Подробнее</p>
          </div>
        </div>
      </div>
  </div>
</template>
<script>
import image from "../assets/img/card.png"
const arr = [
  {
    id: 0,
    title: "Хотите реализовать свой проект?Мы вам поможем!",
    text: "Смотреть инвестиционные проекты, площадки и предложения на карте", 
		img: image,
  },
  {
    id: 1,
    title: 'Конкурс "Лучший городской инновационный проект"',
    text: "Смотреть инвестиционные проекты, площадки и предложения на карте",  
		img: image,
  },
  {
    id: 2,
    title: "Инвестиционная карта города",
    text: "Смотреть инвестиционные проекты, площадки и предложения на карте",  
		img: image,
  },
];
export default {
  data() {
    return {
      arr,
    };
  },
};
</script>
<style lang="sass" scoped>
.container
	max-width: 1410px
	margin: 0 auto
	display: flex
	justify-content: space-between
	align-items: flex-end

.card
	width: 450px
	background: #FFFFFF
	border-radius: 4px 4px 0px 0px
	margin: 0 30px 0 0
	&:last-child
		margin: 0

.head
	padding: 0 55px
	height: 65px
	display: flex
	flex-direction: column
	align-items: center
	& h1
		font-style: normal
		font-weight: 500
		font-size: 20px
		line-height: 24px
		text-align: center
		margin: 0
		color: #000000
.arrow
	margin: 7px 0 5px 0
	content: ''
	width: 12px
	height: 1px
	background: #D43A3F
	transform: rotate(-25deg)
	&::after
		content: ''
		position: absolute
		width: 12px
		height: 1px
		top: 4px
		right: -9px
		background: #D43A3F
		transform: rotate(50deg)

.show__text
	position: relative
	display: none
	& img
		width: 100%
		height: 100%
		object-fit: fill
	& .text
		position: absolute
		bottom: 0
		padding: 4px 6px 8px 6px

		background: rgba(255, 255, 255, 0.9)
		& h1
			font-style: normal
			font-weight: 300
			font-size: 16px
			line-height: 19px

			color: #000000

			padding: 0 0 48px 0

		& p
			text-align: end
			font-style: normal
			font-weight: 500
			font-size: 14px
			line-height: 17px

			color: #D53A3F
			&:hover
				color: green
				transition: all .3s ease-out
.card:hover .show__text
	display: block

@media screen and (max-width: 1410px )
	.container
		margin: 0 15px
	.card
		width: 350px
	.head
		padding: 0 30px
		height: 50px
		display: flex
		flex-direction: column
		align-items: center
		& h1
			font-size: 16px
			line-height: 18px
@media screen and (max-width: 1110px )
	.card
		width: 250px
		height: 40px
	.head
		padding: 0 20px
		height: 35px
		display: flex
		flex-direction: column
		align-items: center
		& h1
			font-size: 12px
			line-height: 18px
	.show__text
		& .text
			position: absolute
			bottom: 0
			padding: 4px 6px 8px 6px

			background: rgba(255, 255, 255, 0.9)
			& h1
				font-size: 12px

				padding: 0 0 20px 0
			& p
				font-size: 10px
				line-height: 17px
				&:hover
					color: green
					transition: all .3s ease-out

</style>