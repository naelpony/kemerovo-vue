<template>
  <form class="form">
    <div class="form__div">
      <input type="text" class="form__input" placeholder=" " />
      <label for="" class="form__label">поиск по сайту</label>
      <span class="img"><icon-search :iconColor="'#484848'"/></span>
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
	position: relative

	&__div
		position: relative
		width: 100%
		height: 30px
		border-bottom: 1px solid #484848

	&__input
		position: absolute
		top: 0
		left: 0
		width: 100%
		height: 100%
		border: none
		border-radius: .5rem
		outline: none
		color: #484848
		background: none
		z-index: 1

	&__label
		position: absolute
		left: 0
		top: 30%

		font-style: normal
		font-weight: 400
		font-size: 14px
		line-height: 150%
		text-transform: uppercase

		color: #484848
		background-color: none
		transition: .3s

.form__input:focus + .form__label
	top: -15px
	left: 0
	color: #484848
	font-weight: 400
	z-index: 10

.img
	position: absolute
	right: 0
	bottom: 0
	display: block
	color: #484848
</style>