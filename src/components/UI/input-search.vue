<template>
  <form class="form">
    <div class="form__div">
      <input type="text" class="form__input" placeholder=" " />
      <label for="" class="form__label">поиск по сайту</label>
			<span class="img"><img src="../../assets/img/search.svg" alt=""></span>
    </div>
  </form>
</template>
<script>
import iconSearch from "../icon/icon-search.vue";
export default {
  components: { iconSearch },
};
</script>
<style lang="sass" scoped>
.form
	width: 100%
	position: relative


	&__div
		position: relative
		width: 100%
		height: 30px
		border-bottom:  1px solid rgba(255, 255, 255, 0.8)

	&__input
		position: absolute
		top: 0
		left: 0
		width: 100%
		height: 100%
		border: none
		border-radius: .5rem
		outline: none
		color: rgba(255, 255, 255, 0.8)
		background: none
		z-index: 1

	&__label
		position: absolute
		left: 0
		top: 30%

		font-style: normal
		font-weight: 300
		font-size: 14px
		line-height: 150%

		text-transform: uppercase

		color: rgba(255, 255, 255, 0.8)
		background-color: none
		transition: .3s

.form__input:focus + .form__label
	top: -15px
	left: 0
	color: rgba(255, 255, 255, 0.8)
	font-weight: 400
	z-index: 10

.img
	position: absolute
	right: 0
	bottom: 0
	display: block
</style>