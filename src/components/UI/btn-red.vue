<template >
  <a href="" class="btn">
    <span class="circl"></span>
    <p>{{name}}</p>
  </a>
</template>
<script>
export default {
	props: {
		name: {
			type: String,
		}
	}
};
</script>
<style lang="sass" scoped>
.btn
	font-style: normal
	font-weight: 500
	font-size: 18px
	line-height: 21px

	color: #D53A3F
	display: flex
	align-items: center
	&:hover
		transition: all .3s ease-out
		color: green

.btn:hover .circl
	transition: all .3s ease-out
	background: url(../../assets/img/arrow.png) green no-repeat center center
.circl
	display: block
	background: url(../../assets/img/arrow.png) #D53A3F no-repeat center center
	border-radius: 50%
	height: 45px
	width: 45px
	margin: 0 15px 0 0
@media screen and (max-width: 1410px )
	.btn
		font-size: 14px
		line-height: 21px

	.circl
		height: 35px
		width: 35px
		margin: 0 10px 0 0
</style>