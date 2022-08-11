<template >
  <div class="logo">
    <div class="logo-image">
      <img src="../../assets/img/logo.png" alt="Кумерово" />
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
</template>
<script>
export default {};
</script>
<style lang="sass" scoped>
.logo
	display: flex
	max-width: 370px
	width: 100%
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
	background-image: url(../../assets/img/cn.png)
	width: 32.35px
	height: 20px
	border: none
	margin: 0 13px 0 0
	padding: 0
.eng
	background-image: url(../../assets/img/eng.png)
	width: 32.35px
	height: 20px
	border: none
	margin: 0 13px 0 0
	padding: 0
.ru
	background-image: url(../../assets/img/ru.png)
	width: 32.35px
	height: 20px
	border: none
	padding: 0
@media screen and (max-width: 1110px )
	.logo
		
	& h2
		font-size: 12px
		line-height: 14px
	& h1
		font-size: 14px
		line-height: 20px
	.logo-image
		margin: 0 10px 0 0
	.title-leng
		display: flex
		align-items: center
		margin: 10px 0 0 0
		& p
			font-size: 10px
			line-height: 10px
	.cn
		background-image: url(../../assets/img/cn.png)
		width: 32.35px
		height: 20px
		border: none
		margin: 0 13px 0 0
		padding: 0
	.eng
		background-image: url(../../assets/img/eng.png)
		width: 32.35px
		height: 20px
		border: none
		margin: 0 13px 0 0
		padding: 0
	.ru
		background-image: url(../../assets/img/ru.png)
		width: 32.35px
		height: 20px
		border: none
		padding: 0
</style>