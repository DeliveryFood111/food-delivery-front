<template>
  <section class="benefitsEnd">
    <div class="benefitsEnd__container">
      <div class="benefitsEnd__cells_content">
        <h4 class="benefitsEnd__cells_chapter">Что мы предлагаем</h4>
        <p class="benefitsEnd__cells_title">Наши лучшие сервисы</p>
        <p class="benefitsEnd__cells_title-text">
          The atmosphere set the stage. It’s about more than just a dining room
          away from your home. food takes the spotlight as guests.
        </p>
      </div>
      <div class="benefitsEnd__container-icons-wrapper">
        <div class="benefitsEnd__cells">
          <div class="benefitsEnd__cells_img">
            <img src="../assets/benefitsEndIcon1.svg" />
          </div>
          <div class="benefitsEnd__cells_text">Открыты 24/7</div>
        </div>
        <div class="benefitsEnd__cells">
          <div class="benefitsEnd__cells_img">
            <img src="../assets/benefitsEndIcon2.svg" />
          </div>
          <div class="benefitsEnd__cells_text">Уникальное меню</div>
        </div>
        <div class="benefitsEnd__cells">
          <div class="benefitsEnd__cells_img">
            <img src="../assets/benefitsEndIcon3.svg" />
          </div>
          <div class="benefitsEnd__cells_text">Доставка на дом</div>
        </div>
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
.benefitsEnd {
  background-color: rgba(41, 46, 54, 1);
  padding: 140px 40px;

  @media screen and (max-width: 993px) {
    justify-content: center;
    padding: 70px 20px 70px;
  }

  &__container {
    display: flex;
    align-items: center;

    @media screen and (max-width: 993px) {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin: 0;
    }

    &-icons-wrapper {
      display: flex;

      @media screen and (max-width: 550px) {
        flex-direction: column;
      }
    }
  }

  &__cells {
    display: flex;
    flex-direction: column;
    border: 20px solid #323841;
    margin-left: 30px;
    padding: 30px 45px;

    @media screen and (max-width: 993px) {
      margin-bottom: 40px;
      align-items: center;
    }

    @media screen and (max-width: 768px) {
      padding: 20px;
    }

    @media screen and (max-width: 550px) {
      margin-left: unset;
    }

    &:first-child {
      margin-left: unset;
    }

    &_img {
      margin-bottom: 15px;
    }

    &_text {
      color: white;
      font-size: 15px;
      font-weight: 400;
    }

    &_content {
      display: flex;
      flex-direction: column;
      margin-right: 50px;

      @media screen and (max-width: 993px) {
        margin-bottom: 30px;
        margin-right: 0;
        width: 400px;
        align-items: center;
        text-align: center;
      }
      @media screen and (max-width: 550px) {
        width: 280px;
      }
    }

    &_chapter {
      color: white;
      width: fit-content;
      font-size: 15px;
      font-weight: 400;
      line-height: 23px;
      letter-spacing: 3px;
      padding-top: 3px;
      padding-bottom: 3px;
      border-bottom: 1px solid #E1B168;
      border-top: 1px solid #E1B168;
    }

    &_title {
      color: white;
      font-size: 40px;
      font-weight: 400;
      line-height: 56px;
    }

    &_title-text {
      color: white;
      font-size: 20px;
      font-weight: 400;
      line-height: 30px;
    }
  }
}
</style>
