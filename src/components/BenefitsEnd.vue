<template>
  <section class="benefits-2">
    <div class="benefits-2__container">
      <div class="benefits-2__cells">
        <div class="benefits-2__cells__img">
          <img src="../assets/benefitsEndIcon1.svg" />
        </div>
        <div class="benefits-2__cells__text">Открыты 24/7</div>
      </div>
      <div class="benefits-2__cells">
        <div class="benefits-2__cells__img">
          <img src="../assets/benefitsEndIcon2.svg" />
        </div>
        <div class="benefits-2__cells__text">Уникальное меню</div>
      </div>
      <div class="benefits-2__cells">
        <div class="benefits-2__cells__img">
          <img src="../assets/benefitsEndIcon3.svg" />
        </div>
        <div class="benefits-2__cells__text">Доставка на дом</div>
      </div>
      <div class="benefits-2__cells__content">
        <h4 class="benefits-2__cells__chapter">Что мы предлагаем</h4>
        <p class="benefits-2__cells__title">Наши лучшие сервисы</p>
        <p class="benefits-2__cells__title-text">
          The atmosphere set the stage. It’s about more than just a dining room
          away from your home. food takes the spotlight as guests. The
          atmosphere set the stage. It’s about more than just a dining room away
          from your home. food takes the spotlight as guests.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BenefitsEnd",
};
</script>

<style scoped lang="scss">
.benefits-2 {
  display: flex;
  flex-direction: row;
  background-color: rgba(41, 46, 54, 1);
  padding: 140px 40px 140px;

  @media screen and (max-width: 993px) {
    justify-content: center;
    padding: 70px 20px 70px;
  }

  &__container {
    display: flex;
    flex-direction: row-reverse;
    align-items: center;

    @media screen and (max-width: 993px) {
      display: flex;
      flex-direction: column-reverse;
      align-items: center;
      margin: 0;
    }
  }

  &__cells {
    display: flex;
    flex-direction: column;
    border: 20px solid #323841;
    width: fit-content;
    height: fit-content;
    margin-left: 30px;
    padding: 30px 45px;

    @media screen and (max-width: 993px) {
      width: 300px;
      align-items: center;
      margin-right: 0;
      margin-left: 0;
      margin-bottom: 40px;
    }

    @media screen and (max-width: 550px) {
      width: 200px;
      padding: 20px;
    }

    &__img {
      margin-bottom: 5px;
    }

    &__text {
      color: white;
      font-size: 15px;
    }

    &__content {
      display: flex;
      flex-direction: column;
      margin-right: 50px;

      @media screen and (max-width: 993px) {
        width: 400px;
        margin-bottom: 30px;
        align-items: center;
        margin-right: 0;
      }
      @media screen and (max-width: 550px) {
        width: 280px;
      }
    }

    &__chapter {
      color: white;
      width: fit-content;
      font-size: 20px;
      font-weight: 900;
      padding-top: 3px;
      padding-bottom: 3px;
      border-bottom: 1px solid yellow;
      border-top: 1px solid yellow;
    }

    &__title {
      color: white;
      font-size: 30px;
    }

    &__title-text {
      color: white;
    }
  }
}
</style>
