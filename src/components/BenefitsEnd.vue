<template>
  <section class="benefitsEnd">
    <div class="benefitsEnd__container">
      <div class="benefitsEnd__cells">
        <div class="benefitsEnd_cells_img">
          <img src="../assets/benefitsEndIcon1.svg" />
        </div>
        <div class="benefitsEnd__cells_text">Открыты 24/7</div>
      </div>
      <div class="benefitsEnd__gicells">
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
      <div class="benefitsEnd__cells_content">
        <h4 class="benefitsEnd__cells_chapter">Что мы предлагаем</h4>
        <p class="benefitsEnd__cells_title">Наши лучшие сервисы</p>
        <p class="benefitsEnd__cells_title-text">
          The atmosphere set the stage. It’s about more than just a dining room
          away from your home. food takes the spotlight as guests.
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
.benefitsEnd{
  display: flex;
  flex-direction: row;
  background-color: rgba(41, 46, 54, 1);
  padding: 140px 40px;

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
        width: 400px;
        margin-bottom: 30px;
        align-items: center;
        margin-right: 0;
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
      border-bottom: 1px solid yellow;
      border-top: 1px solid yellow;
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
