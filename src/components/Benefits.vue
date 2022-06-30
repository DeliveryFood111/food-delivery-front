<template>
  <section class="benefits">
    <div class="benefits__container">
      <div class="benefits__cells">
        <div class="benefits__cells-icon">
          <img src="../assets/location-icon.svg" />
        </div>
        <div class="benefits__cells-text">
          <h4 class="benefits__cells-title">Мы находимся</h4>
          <p class="benefits__cells-p">г.Киев ул.Крещатик 1</p>
        </div>
      </div>
      <div class="benefits__cells">
        <div class="benefits__cells-icon">
          <img src="../assets/scedual-icon.svg" />
        </div>
        <div class="benefits__cells-text">
          <h4 class="benefits__cells-title">Часы работы</h4>
          <p class="benefits__cells-p">Понедельника-Пятницу с 9:00-21:00</p>
        </div>
      </div>
      <div class="benefits__cells">
        <div class="benefits__cells-icon">
          <img src="../assets/reserve-icon.svg" />
        </div>
        <div class="benefits__cells-text">
          <h4 class="benefits__cells-title">Зарезервировать</h4>
          <p class="benefits__cells-p">restaurantate@gmail.com</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Benefits",
};
</script>

<style scoped lang="scss">
.benefits {
  height: auto;
  width: auto;
  background-color: rgba(255, 248, 245, 1);

  &__container {
    display: flex;
    justify-content: space-around;

    @media screen and (max-width: 993px) {
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
  }
  &__cells {
    display: flex;
    padding: 20px;
    align-items: center;

    @media screen and (max-width: 993px) {
      width: 420px;
      justify-content: flex-start;
    }
    @media screen and (max-width: 426px) {
      flex-direction: column;
      text-align: center;
      width: auto;
    }
  }
  &__cells-icon {
    text-align: center;
  }
  &__cells-text {
    display: flex;
    flex-direction: column;
    padding-left: 20px;

    @media screen and (max-width: 992px) {
      align-items: center;
    }
    @media screen and (max-width: 426px) {
      padding-left: 0;
    }
  }
  &__cells-title {
    margin-top: 20px;
    font-weight: 500;
  }
  &__cells-p {
    word-break: break-word;
    margin-top: 5px;
  }
}
</style>
