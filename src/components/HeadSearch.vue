<template>
  <div class="container">
		<logo/>
    <div class="search">
      <input-search />
      <icon-eye width="20" hieght="20" iconName="eye" />
    </div>
  </div>
</template>
<script>
import IconEye from "./icon/icon-eye.vue";
import InputSearch from "./UI/input-search.vue";
import Logo from './UI/logo.vue';
export default {
  components: { IconEye, InputSearch, Logo },
};
</script>
<style lang="sass" scoped>
.container
	margin: 17px auto 20px auto
	max-width: 1410px
	display: flex
	flex-grow: 0
.search
	display: flex
	align-items: center
	width: 100%
	margin: 25px 0 0 21px
@media screen and (max-width: 1410px )
	.container
		margin: 10px 15px

</style>