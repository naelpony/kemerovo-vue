<template >
  <div class="container">
    <div class="section">
      <h1>КЕМЕРОВО</h1>
      <h2>город возможностей</h2>
      <div class="section-icon">
        <div class="icon">
          <img src="../assets/img/strongbox.svg" alt="" />
          <p class="icon-title">Банк бережливых технологий</p>
        </div>
        <div class="icon">
          <img src="../assets/img/courthouse.svg" alt="" />
          <p class="icon-title">Столица Кузбасса</p>
        </div>
        <div class="icon">
          <img src="../assets/img/people.svg" alt="" />
          <p class="icon-title">
            Первый по численности населения город в Кемеровской области
          </p>
        </div>
        <div class="icon">
          <img src="../assets/img/award.svg" alt="" />
          <p class="icon-title">Истории успеха</p>
        </div>
      </div>
      <div class="section-icon-mobil">
        <div class="mobil-left">
          <div class="icon">
            <img src="../assets/img/strongbox.svg" alt="" />
            <p class="icon-title">Банк бережливых технологий</p>
          </div>
          <div class="icon">
            <img src="../assets/img/courthouse.svg" alt="" />
            <p class="icon-title">Столица Кузбасса</p>
          </div>
        </div>
        <div class="mobil-right">
          <div class="icon">
            <img src="../assets/img/people.svg" alt="" />
            <p class="icon-title">
              Первый по численности населения город в Кемеровской области
            </p>
          </div>
          <div class="icon">
            <img src="../assets/img/award.svg" alt="" />
            <p class="icon-title">Истории успеха</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import IconAward from "./icon/icon-award.vue";
import IconCourthouse from "./icon/icon-courthouse.vue";
import IconPeople from "./icon/icon-people.vue";
import iconStrongbox from "./icon/icon-strongbox.vue";
export default {
  components: { iconStrongbox, IconPeople, IconCourthouse, IconAward },
};
</script>
<style lang="sass" scoped>
.section-icon-mobil
	display: none

.container
	position: relative
	background: linear-gradient(180deg, rgba(255, 255, 255, 0) 0%, rgba(255, 255, 255, 0.4) 50.56%, rgba(255, 255, 255, 0) 100%)
	backdrop-filter: blur(2px)
	z-index: -1
	margin: 177px 0 0 0
.section
	display: flex
	flex-direction: column
	align-items: center
	margin: 0 auto
	max-width: 1410px
h1
	font-style: normal
	font-weight: 700
	font-size: 36px
	line-height: 43px
	letter-spacing: 0.02em
	margin: 0
	padding: 0 0 4px 0
	color: #FFFFFF
h2
	font-style: normal
	font-weight: 400
	font-size: 20px
	line-height: 24px
	letter-spacing: 0.02em
	margin: 0
	padding: 0 0 56px 0

	color: #FFFFFF
.section-icon
	display: flex
	justify-content: space-between
	align-items: center
	width: 994px
.icon
	display: flex
	flex-direction: column
	align-items: center
	align-self: flex-start
	max-width: 236px
	&:first-child
		max-width: 164px
p
	font-style: normal
	font-weight: 500
	font-size: 14px
	line-height: 17px
	letter-spacing: 0.02em
	text-align: center

	color: #F4F4F4
@media screen and (max-width: 1410px )
	.container
		margin: 100px 0 0 0
	img
		width: 40px
		height: 40px
	h1
		font-size: 36px
		line-height: 20px
	h2
		font-size: 16px
		line-height: 20px
	.section-icon
		display: flex
		justify-content: space-between
		align-items: center
		width: 700px
	p
		font-size: 12px
		line-height: 12px
@media screen and (max-width: 810px )
	.container
		margin: 150px 0 0 0
	img
		width: 30px
		height: 30px
	h1
		font-size: 28px
		line-height: 20px
	h2
		font-size: 16px
		line-height: 20px
	.section-icon
		display: flex
		justify-content: space-between
		align-items: center
		width: 100%
	p
		font-size: 12px
		line-height: 12px
	.section
		max-width: 550px
@media screen and (max-width: 425px )
	.section-icon
		display: none
	.section-icon-mobil
		display: flex
</style>