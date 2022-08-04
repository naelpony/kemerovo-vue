<template>
	<form>
		<input type="text" class="input">
	</form>
</template>
<script>
import iconSearch from '../icon/icon-search.vue'
export default {
  components: { iconSearch },
	
}
</script>
<style lang="sass">
.input
	width: 845px
	background: url('../../assets/img/search.svg') no-repeat
	background-position: 100% 0
	border: none
	border-bottom: 1px solid rgba(255, 255, 255, 0.8)
	&:focus			
		outline: none
	&:hover
</style>