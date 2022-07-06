<template>
  <section class="history-images">
    <h3 class="history-images__topic">История основных блюд</h3>
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
        <h4 class="history-images__title">Борщ</h4>
        <p class="history-images__content">
          Горячий заправочный суп на основе свёклы,которая придаёт ему
          характерный красный цвет. В словаре В. И. Даля — род щей, похлёбка из
          квашеной свёклы, на говядине и свинине, или со свиным салом.
          Традиционное блюдо восточных славян, основное первое блюдо украинской
          кухни.
        </p>
      </div>
    </div>
    <div class="history-images__container container_vareniki">
      <img
        class="history-images__img"
        src="../assets/vareniki.webp"
        alt="Vareniki"
      />
      <div class="history-images__text">
        <h4 class="history-images__title">Вареники</h4>
        <p class="history-images__content content_vareniki">
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
        <h4 class="history-images__title">Салатик</h4>
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
  padding: 84px 54px 125px 40px;
  background-color: rgba(255, 248, 245, 1);
  display: flex;
  width: fit-content;
  flex-direction: column;

  &__topic {
    text-align: center;
    margin-bottom: 35px;
    font-size: xx-large;
    text-shadow: 1px 3px 5px grey;

    @media screen and (max-width: 993px) {
      margin-bottom: 10px;
    }

    @media screen and (max-width: 550px) {
      font-size: x-large;
    }
  }
  &__description {
    text-indent: 20px;
    margin-bottom: 40px;
    font-size: 15px;

    @media screen and (max-width: 993px) {
      margin-bottom: 20px;
    }
  }
  &__container {
    display: flex;
    flex-direction: row;
    margin-bottom: 20px;

    @media screen and (max-width: 993px) {
      flex-direction: column;
      align-items: center;
      margin-bottom: 40px;
    }
  }
  &__img {
    border-radius: 1%;
    width: 650px;
    height: 500px;
    padding-bottom: 20px;

    @media screen and (max-width: 993px) {
      width: 450px;
      height: auto;
    }

    @media screen and (max-width: 550px) {
      width: 300px;
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
    margin: auto 0;
  }
  &__title {
    display: flex;
    justify-content: center;
    font-size: x-large;
    margin-bottom: 30px;
    letter-spacing: 20px;

    @media screen and (max-width: 993px) {
      margin-bottom: 0;
    }

    @media screen and (max-width: 550px) {
      letter-spacing: 5px;
    }
  }
  &__content {
    display: flex;
    text-indent: 20px;
    font-size: 20px;
    margin-left: 30px;

    @media screen and (max-width: 550px) {
      margin-left: 0;
    }
  }
}
.container_vareniki {
  display: flex;
  flex-direction: row-reverse;

  @media screen and (max-width: 993px) {
    flex-direction: column;
    align-items: center;
    margin-bottom: 40px;
  }
}
.content_vareniki {
  margin-right: 20px;

  @media screen and (max-width: 993px) {
    margin-right: 0;
  }
}
</style>
