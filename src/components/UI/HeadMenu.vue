<template>
  <div class="container">
    <nav class="menu">
      <ul class="menu__list">
        <li>
          <a href="" class="menu__link">О Кемерово</a>
          <ul class="sabmenu__list">
            <li>
              <a href="" class="sabmenu__link"
                >Обращение главы города Кемерово</a
              >
            </li>
            <li>
              <a href="" class="sabmenu__link"
                >Стратегия социально-экономического развития города</a
              >
            </li>
          </ul>
        </li>
        <li>
          <a href="" class="menu__link">Малому бизнесу</a>
          <ul class="sabmenu__list">
            <li>
              <a href="" class="sabmenu__link"
                >Обращение главы города Кемерово</a
              >
            </li>
            <li>
              <a href="" class="sabmenu__link"
                >Стратегия социально-экономического развития города</a
              >
            </li>
          </ul>
        </li>
        <li>
          <a href="" class="menu__link">Инвестору</a>
          <ul class="sabmenu__list">
            <li>
              <a href="" class="sabmenu__link"
                >Обращение главы города Кемерово</a
              >
            </li>
            <li>
              <a href="" class="sabmenu__link"
                >Стратегия социально-экономического развития города</a
              >
            </li>
          </ul>
        </li>
        <li>
          <a href="" class="menu__link">Меры поддержки</a>
          <ul class="sabmenu__list">
            <li>
              <a href="" class="sabmenu__link"
                >Обращение главы города Кемерово</a
              >
            </li>
            <li>
              <a href="" class="sabmenu__link"
                >Стратегия социально-экономического развития города</a
              >
            </li>
          </ul>
        </li>
        <li>
          <a href="" class="menu__link">Инвестиционная деятельность</a>
          <ul class="sabmenu__list">
            <li>
              <a href="" class="sabmenu__link"
                >Обращение главы города Кемерово</a
              >
            </li>
            <li>
              <a href="" class="sabmenu__link"
                >Стратегия социально-экономического развития города</a
              >
            </li>
          </ul>
        </li>
        <li>
          <a href="" class="menu__link">ОРВ</a>
        </li>
        <li>
          <a href="" class="menu__link">Обратная связь</a>
        </li>
      </ul>
    </nav>
  </div>
</template>
<script>
export default {};
</script>
<style lang="sass" scoped>
.container
  background: rgba(160, 47, 50, 0.8)
.menu
  max-width: 1410px
  margin: 0 auto
  display: flex
  align-items: center
  justify-content: center
a
  text-decoration: none
li
  position: relative
  list-style: none
.menu__list
  display: flex
  align-items: center
  padding: 0
  margin: 0
.menu__list>li
  padding: 8px 52px 8px 0
.menu__list>li:hover
  background: green
.menu__list>li:hover .sabmenu__list
  display: block
.menu__link
  padding: 0
  font-weight: 300
  font-size: 20px
  line-height: 24px
  letter-spacing: 0.02em
  color: #E7E7E7
.sabmenu__list
  display: none
  position: absolute
  left: 0
  top: 12px
  padding: 20px 0 0 0
  width: 100%
  border-radius: 0px 0px 2px 2px
.sabmenu__list>li

  background: #FFFFFF
  text-align: center

  padding: 9px 7px
.sabmenu__list>li:hover
  background: #B8B3B3
.sabmenu__link
  font-style: normal
  font-weight: 400
  font-size: 12px
  line-height: 14px
  letter-spacing: 0.02em

  color: #484848

@media screen and (max-width: 1410px )
  .menu
    margin: 0 15px
  .menu__link
    padding: 0
    font-weight: 300
    font-size: 16px
    line-height: 18px
    letter-spacing: 0.02em
    color: #E7E7E7
  .sabmenu__link
    font-style: normal
    font-weight: 400
    font-size: 8px
    line-height: 10px
    letter-spacing: 0.02em

    color: #484848
  .menu__list>li
    padding: 8px 30px 8px 0
</style>