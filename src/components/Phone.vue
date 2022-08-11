<template >
  <div class="container">
    <div class="logo">
      <img src="../assets/img/logo.png" alt="" />
      <div class="title">
        <h2>Инвестиционный портал</h2>
        <h1>города Кемерово</h1>
      </div>
      <div class="language">
        <select>
          <option>CH</option>
          <option>ENG</option>
          <option selected>RU</option>
        </select>
      </div>
    </div>
    <div class="search">
      <input-search />
    </div>
  </div>
</template>
<script>
import inputSearch from "./UI/input-search.vue";
export default {
  components: { inputSearch },
};
</script>
<style lang="sass" scoped>
.container
	display: flex
	margin: 10px 15px
	width: 100%
	align-items: center
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

.search

	padding: 0 10px 0 0
	width: 100%
@media screen and (max-width: 425px )
	.container
		flex-direction: column
	.logo
		max-width: 100%
		& img
			width: 20%
	.title
		margin: 0 10px 0 0
</style>