<template>
  <div class="cantainer">
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
<style lang="sass">
.cantainer
  background: rgba(160, 47, 50, 0.8)
  display: flex
  align-items: center
  height: 40px
.menu
  margin: 0 auto
  width: 100%
  max-width: 1410px
a
  text-decoration: none
li
  position: relative
  list-style: none
.menu__list
  display: flex
  align-items: center
  padding: 0
.menu__list>li:hover .sabmenu__list
  display: block
.menu__link
  padding: 0 52px 0 0
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
.sabmenu__link
  font-style: normal
  font-weight: 400
  font-size: 12px
  line-height: 14px
  letter-spacing: 0.02em

  color: #484848
</style>