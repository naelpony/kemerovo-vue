<template >
  <div class="container">
    <h1>Удобно ли Вам работать с нашим сайтом?</h1>
    <form class="form" @submit.prevent>
      <label class="form-control">
        <input type="radio" name="radio" />
        Да | 40 голосов
      </label>

      <label class="form-control">
        <input type="radio" name="radio" />
        Нет | 31 голосов
      </label>
      <button type="submit" class="submit">Отправить</button>
    </form>
  </div>
</template>
<script>
export default {};
</script>
<style lang="sass" scoped>
.container
	max-width: 1410px
	margin: 0 auto
	display: flex
	flex-direction: column
	align-items: center
	padding: 62px 0 0 0
	& h1
		font-style: normal
		font-weight: 400
		font-size: 20px
		line-height: 150%

		color: #484848

.form
	display: flex
	align-items: flex-start
	flex-direction: column
	font-style: normal
	font-weight: 400
	font-size: 20px
	line-height: 150%

	color: #484848
.form-control
	display: flex
	align-items: center
	margin: 35px 0 0 0
input[type="radio"]
	appearance: none
	margin: 0 26px 0 0
	color: #484848
	width: 24px
	height: 24px
	border: 1px solid #484848
	border-radius: 50%
	transform: translateY(-0.1px)
	display: grid
	place-content: center

input[type="radio"]::before
	content: ''
	width: 16px
	height: 16px
	border-radius: 50%
	transform: scale(0)
	transition: 120ms transform ease-in-out
	box-shadow: inset 1em 1em #484848
input[type="radio"]:checked::before
	transform: scale(1)

.submit
	margin: 20px 0 0 0
	font-style: normal
	font-weight: 400
	font-size: 18px
	line-height: 150%

	display: flex
	align-items: center
	text-align: center

	color: #FFFFFF
	padding: 10px 29px
	background: #D43A3F
	border: none
	border-radius: 40px

@media screen and (max-width: 1410px )

	.container
		margin: 0 15px
		padding: 32px 0 0 0
		& h1
			font-size: 18px

	.form
		font-size: 18px
	.form-control
		display: flex
		align-items: center
		margin: 17px 0 0 0
	input[type="radio"]
		appearance: none
		margin: 0 20px 0 0
		width: 18px
		height: 18px

	input[type="radio"]::before
		width: 10px
		height: 10px
	input[type="radio"]:checked::before
		transform: scale(1)

	.submit
		margin: 16px 0 0 16px
		font-size: 14px
</style>