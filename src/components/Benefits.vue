<template>
  <section class="benefits">
    <div class="benefits__container">
      <div class="benefits__cells">
        <div class="benefits__cells-icon">
          <img src="../assets/location-icon.svg" />
        </div>
        <div class="benefits__cells-text">
          <h4 class="benefits__cells-title">Быстро доставим!</h4>
          <p class="benefits__cells-p">Доставляем еду в течении 30 минут</p>
        </div>
      </div>
      <div class="benefits__cells">
        <div class="benefits__cells-icon">
          <img src="../assets/scedual-icon.svg" />
        </div>
        <div class="benefits__cells-text">
          <h4 class="benefits__cells-title">Часы работы</h4>
          <p class="benefits__cells-p">Работаем 24/7</p>
        </div>
      </div>
      <div class="benefits__cells">
        <div class="benefits__cells-icon">
          <img src="../assets/reserve-icon.svg" />
        </div>
        <div class="benefits__cells-text">
          <h4 class="benefits__cells-title">Простота оформления</h4>
          <p class="benefits__cells-p">Оформляй заказ быстро и легко</p>
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
  padding-top: 100px;
  padding-bottom: 60px;
  height: auto;
  width: auto;
  background-color: rgba(255, 248, 245, 1);

  @media screen and (max-width: 993px) {
    padding-top: 60px;
  }

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
