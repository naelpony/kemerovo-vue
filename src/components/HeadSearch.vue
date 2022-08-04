<template>
  <div class="container">
    <div class="logo">
      <div class="logo-image">
        <img src="../assets/img/logo.png" alt="Кумерово" />
      </div>
      <div class="logo-title">
        <h2>Инвестиционный портал</h2>
        <h1>города Кемерово</h1>
        <div class="title-leng">
          <p>доступно на языках:</p>
          <div class="leng">
            <button class="cn"></button>
            <button class="eng"></button>
            <button class="ru"></button>
          </div>
        </div>
      </div>
    </div>
    <div class="search">
      <input-search />
      <icon-eye width="20" hieght="20" iconName="eye" />
    </div>
  </div>
</template>
<script>
import IconEye from "./icon/icon-eye.vue";
import InputSearch from "./UI/input-search.vue";
export default {
  components: { IconEye, InputSearch },
};
</script>
<style lang="sass">
.container
	margin: 17px auto 20px auto
	max-width: 1410px
	display: flex
	align-items: center
.logo
	display: flex
	& h2
		font-style: normal
		font-weight: 300
		font-size: 14px
		line-height: 17px
		color: #FFFFFF
		margin: 0
	& h1
		font-style: normal
		font-weight: 800
		font-size: 20px
		line-height: 24px
		letter-spacing: 0.02em
		color: #E7E7E7
		margin: 0
.logo-image
	margin: 0 30px 0 0
.title-leng
	display: flex
	align-items: center
	margin: 10px 0 0 0
	& p
		font-style: normal
		font-weight: 300
		font-size: 12px
		line-height: 14px
		color: #E7E7E7
		margin: 0 11px 0 0

.cn
	background-image: url(../assets/img/cn.png)
	width: 32.35px
	height: 20px
	border: none
	margin: 0 13px 0 0
	padding: 0
.eng
	background-image: url(../assets/img/eng.png)
	width: 32.35px
	height: 20px
	border: none
	margin: 0 13px 0 0
	padding: 0
.ru
	background-image: url(../assets/img/ru.png)
	width: 32.35px
	height: 20px
	border: none
	padding: 0

.search
	display: flex
	align-items: center

	margin: 25px 0 0 21px
</style>