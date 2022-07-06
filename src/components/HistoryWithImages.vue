<template>
  <section class="history-images">
    <h2 class="history-images__topic">История основных блюд</h2>
    <p class="history-images__description">
      Главное блюдо обычно самое тяжёлое, горячее и самое сложное блюдо в меню.
      Основными ингредиентами являются мясо или рыба. В вегетарианской кухне
      роль главного играют обычно блюда из бобовых. Главному блюду предшествует
      закуска, суп и (или) салат, а после него — десерт.
    </p>
    <div class="history-images__container">
      <img
        class="history-images__img"
        src="../assets/ukraine-borsch.webp"
        alt="Borshch"
      />
      <div class="history-images__text">
        <h3 class="history-images__title">Борщ</h3>
        <p class="history-images__content">
          Горячий заправочный суп на основе свёклы,которая придаёт ему
          характерный красный цвет. В словаре В. И. Даля — род щей, похлёбка из
          квашеной свёклы, на говядине и свинине, или со свиным салом.
          Традиционное блюдо восточных славян, основное первое блюдо украинской
          кухни.
        </p>
      </div>
    </div>
    <div class="history-images__container container_reversed">
      <img
        class="history-images__img"
        src="../assets/vareniki.webp"
        alt="Vareniki"
      />
      <div class="history-images__text">
        <h3 class="history-images__title">Вареники</h3>
        <p class="history-images__content content_reversed">
          Варе́ники — украинское национальное блюдо в виде отварных изделий из
          пресного теста с начинкой из отварного мяса, овощей, грибов, фруктов,
          творога, картофеля и ягод. Вареники в XIX веке были известны также
          крестьянам Курской губернии. Сходно с марийским блюдом подкогыльо.
        </p>
      </div>
    </div>
    <div class="history-images__container">
      <img class="history-images__img" src="../assets/salad.webp" alt="Salad" />
      <div class="history-images__text">
        <h3 class="history-images__title">Салат</h3>
        <p class="history-images__content">
          Сала́т - холодное блюдо из кусочков овощей, зелени, различных других
          растений, грибов, с добавлением приправы. Салатом считается любое
          сочетание ингредиентов, имеющее заправку или приправу, либо и то, и
          другое.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HistoryWithImages",
};
</script>

<style scoped lang="scss">
.history-images {
  padding: 34px 54px 125px 40px;
  background-color: rgba(255, 248, 245, 1);
  display: flex;
  width: fit-content;
  flex-direction: column;

  &__topic {
    margin-bottom: 8px;
    font-size: 40px;
    font-weight: 400;
    line-height: 56px;
    text-align: center;
  }

  &__description {
    margin-bottom: 50px;
    font-size: 20px;
    font-weight: 400;
    line-height: 30px;
  }

  &__container {
    display: flex;
    flex-direction: row;
    margin-bottom: 80px;

    &:last-child {
      margin-bottom: unset;
    }

    @media screen and (max-width: 993px) {
      margin-bottom: 40px;
    }

    @media screen and (max-width: 750px) {
      flex-direction: column;
      align-items: center;
    }
  }

  &__img {
    border-radius: 1%;
    width: 743px;
    height: 519px;
    padding-bottom: 20px;

    @media screen and (max-width: 1150px) {
      width: 643px;
      height: 419px;
    }

    @media screen and (max-width: 993px) {
      width: 450px;
      height: 419px;
    }

    @media screen and (max-width: 830px) {
      width: 300px;
      height: 319px;
    }

    @media screen and (max-width: 430px) {
      width: 250px;
    }

    @media screen and (max-width: 361px) {
      width: 200px;
    }
  }

  &__text {
    display: flex;
    flex-direction: column;
    margin-left: 45px;

    @media screen and (max-width: 750px) {
      flex-direction: column;
      align-items: center;
      margin-left: unset;
    }
  }

  &__title {
    margin-bottom: 30px;
    font-size: 40px;
    font-weight: 400;
    line-height: 56px;

    @media screen and (max-width: 993px) {
      margin-bottom: 0;
    }
  }

  &__content {
    display: flex;
    font-size: 20px;
    font-weight: 400;
    line-height: 30px;

    @media screen and (max-width: 550px) {
      margin-left: 0;
    }
  }
}
.container_reversed {
  display: flex;
  flex-direction: row-reverse;

  & > .history-images__text {
    margin-right: 45px;

    @media screen and (max-width: 750px) {
      margin-right: unset;
    }
  }

  @media screen and (max-width: 993px) {
    margin-bottom: 40px;
  }

  @media screen and (max-width: 750px) {
    flex-direction: column;
    align-items: center;
  }
}
.content_reversed {
  margin-right: 20px;

  @media screen and (max-width: 993px) {
    margin-right: 0;
  }
}
</style>
