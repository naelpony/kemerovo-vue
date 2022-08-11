<template >
  <div class="name">
    <span class="line"></span>
    <p>{{ name }}</p>
  </div>
</template>
<script>
export default {
  props: {
    name: {
      type: String,
    },
  },
};
</script>
<style lang="sass" scoped>
.name
	position: relative
	min-width: 100%
	& p
		font-style: normal
		font-weight: 700
		font-size: 48px
		line-height: 57px
		text-transform: uppercase
		padding: 0 0 0 24px
		color: #212121

.line
	content: ' '
	position: absolute
	width: 4px
	height: 100%
	background: #D53A3F
	border-radius: 1px

@media screen and (max-width: 1410px )
	.name
		position: relative
		min-width: 100%
		& p
			font-size: 34px
			line-height: 40px
			text-transform: uppercase
			padding: 0 0 0 18px
			color: #212121

	.line
		content: ' '
		position: absolute
		width: 4px
		height: 100%
		background: #D53A3F
		border-radius: 1px
</style>