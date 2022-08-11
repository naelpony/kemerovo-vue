<template >
  <div class="container">
    <title-name :name="'Обращение Главы города Кемерово'" />
    <div class="contetn">
      <div class="title">
        <span class="text">
          <p>
            В последние годы Кузбасс динамично развивается. Флагманом позитивных
            перемен является столица региона – город Кемерово. Именно здесь
            происходят главные события в культурной, научной, деловой и
            спортивной сферах. Кемерово – город большой химии, в котором
            работают передовые предприятия этой отрасли. Также наш город
            является транспортным центром с международным аэропортом и
            железнодорожным узлом.
          </p>
          <p>
            На протяжении многих лет Кемерово лидирует среди кузбасских городов
            по объему инвестиций и количеству субъектов малого и среднего
            предпринимательства. Бизнесмены выбирают наш город из-за
            благоприятных условий для запуска своего дела и инвестирования в
            различные сферы. Особенно в такие, как модернизация действующих
            производств, строительство жилья, дорог и объектов социальной сферы.
          </p>
          <p>
            В прошлом году Кузбасс отметил большой праздник – 300-летие
            промышленного освоения региона...
          </p>
        </span>
        <div class="btn">
          <btn-red :name="'Подробнее'" />
        </div>
      </div>
      <div class="image">
        <img src="../assets/img/about.png" alt="" />
      </div>
    </div>
  </div>
</template>
<script>
import titleName from "./UI/title-name.vue";
import btnRed from "./UI/btn-red.vue";

export default {
  components: {
    titleName,
    btnRed,
  },
};
</script>
<style lang="sass" scoped>
.container
  max-width: 1410px
  margin: 240px auto 0 auto
.contetn
  display: flex
  justify-content: space-between
  margin: 60px 0 0 0
  position: relative
.title
  max-width: 600px
.text
  font-style: normal

  font-weight: 300
  font-size: 18px
  line-height: 150%
  color: #9E9E9E
.btn
  margin: 87px 0 0 0
@media screen and (max-width: 1410px )
  .container
    margin: 100px 15px 0 15px
  .contetn
    margin: 40px 0 0 0
  .text
    font-size: 16px
    line-height: 100%
  .btn
    margin: 67px 0 0 0
  img
    width: 400px
@media screen and (max-width: 1110px )
  .container
    margin: 100px 15px 0 15px
  .contetn
    margin: 40px 0 0 0
  .title
    margin: 0 10px 0 0
  .text
    font-size: 16px
    line-height: 100%
  .btn
    margin: 67px 0 0 0
  img
    width: 400px
@media screen and (max-width: 810px )
  .contetn
    margin: 20px auto 0 auto
    max-height: 450px
  .title
    position: absolute
    top: 0
    left: 0
    z-index: 3
    background: rgba(255, 255, 255, 0.6)
    width: 70%
    padding: 10px
    height: 100%
  .text
    font-size: 14px
    line-height: 100%
    color: #000000
  img

    width: 100%
    height: 100%

    object-fit: cover
@media screen and (max-width: 425px )
  .contetn
    min-height: 500px
  .title
    width: 95%
  .image
    min-width: 100%
  .btn
    margin: 10px 0 0 0
</style>