<template >
  <div class="container">
    <title-name :name="'Новости портала'" />
    <div class="news">
      <div class="news__item" v-for="items in arr" :key="items.id">
        <img :src="items.img" />
        <div class="item__text">
          <span>{{ items.date }}</span>
          <p>{{ items.paragraf }}</p>
        </div>
      </div>
    </div>
    <div class="bt">
      <btn-red :name="'Все новости'" />
    </div>
  </div>
</template>
<script>
import titleName from "./UI/title-name.vue";
import btnRed from "./UI/btn-red.vue";
import pic1 from "../assets/img/pic1.png";
import pic2 from "../assets/img/pic2.png";
import pic3 from "../assets/img/pic3.png";

const arr = [
  {
    id: 0,
    date: "30.05.2022",
    paragraf: "С днем российского предпринимательства!",
    img: pic1,
  },
  {
    id: 1,
    date: "26.05.2022",
    paragraf:
      "Фонд социального страхования сообщает о возможности снизить расходы на реализацию мер по сокращению производственного травматизма и профессиональных заболеваний за счет средств обязательного социального страхования",
    img: pic2,
  },
  {
    id: 2,
    date: "23.05.2022",
    paragraf:
      "Вебинар для предпринимателей о мерах их поддержки и преимуществах использования бизнесом Системы быстрых платежей (24.05.2022)",
    img: pic3,
  },
  {
    id: 3,
    date: "23.05.2022",
    paragraf:
      "Вебинар для предпринимателей о мерах их поддержки и преимуществах использования бизнесом Системы быстрых платежей (24.05.2022)",
    img: pic3,
  },
  {
    id: 4,
    date: "23.05.2022",
    paragraf:
      "Вебинар для предпринимателей о мерах их поддержки и преимуществах использования бизнесом Системы быстрых платежей (24.05.2022)",
    img: pic2,
  },
  {
    id: 5,
    date: "30.05.2022",
    paragraf:
      "Фонд социального страхования сообщает о возможности снизить расходы на реализацию мер по сокращению производственного травматизма и профессиональных заболеваний за счет средств обязательного социального страхования",
    img: pic1,
  },
];

export default {
  data() {
    return {
      arr,
    };
  },
  components: {
    titleName,
    btnRed,
  },
};
</script>
<style lang="sass" scoped>
.container
  max-width: 1410px
  margin: 153px auto 0 auto

.news
  display: flex
  flex-wrap: wrap
  justify-content: space-between
  margin: 30px 0 0 0
.news__item
  position: relative
  margin: 30px 0 0 0
.item__text
  position: absolute
  bottom: 0
  min-height: 176px

  background: rgba(255, 255, 255, 0.9)
  backdrop-filter: blur(4px)

  border-radius: 4px
  & span
    font-weight: 400
    font-size: 14px
    line-height: 17px

    color: #484848

    display: flex
    justify-content: flex-end
    padding: 10px 5px 12px 0
  & p
    font-weight: 300
    font-size: 16px
    line-height: 19px
    padding: 0 11px
img
  border-radius: 4px
.bt
  display: flex
  justify-content: flex-end
  margin: 65px 0 0 0
  padding: 0
@media screen and (max-width: 1410px )
  .container
    margin: 100px 15px 0 15px

  .news
    justify-content: center
  .news__item
    width: 400px
    margin: 20px 20px 0 0
  .item__text
    min-height: 146px
    width: 100%
    & span
      padding: 8px 5px 10px 0
    & p
      padding: 0 11px
  img
    width: 100%
    height: 100%

    object-fit: cover
    border-radius: 4px
  .bt
    display: flex
    justify-content: flex-end
    margin: 40px 0 0 0
    padding: 0
@media screen and (max-width: 1110px )
  .container
    margin: 100px 15px 0 15px

  .news
    justify-content: center
  .news__item
    width: 300px
    margin: 20px 20px 0 0
  .item__text
    min-height: 146px
    width: 100%
    & span
      font-size: 10px
    & p
      font-size: 12px
  img
    width: 100%
    height: 100%

    object-fit: cover
    border-radius: 4px
  .bt
    display: flex
    justify-content: flex-end
    margin: 40px 0 0 0
    padding: 0
</style>