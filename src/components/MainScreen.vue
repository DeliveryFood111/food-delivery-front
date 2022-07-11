<template>
  <section class="main-screen">
    <div class="main-screen__info">
      <h1>
        Доставка їжі
      </h1>
      <p>
        Доставка збалансованого денного раціону до вашого будинку
      </p>
      <button class="btn btn-dark" type="button">
        Перейти в меню
      </button>
    </div>
    <div class="main-screen__image">
      <img src="../assets/main-screen-image.jpeg">
    </div>
  </section>
</template>

<script>
export default {
  name: "MainScreen"
};
</script>

<style scoped lang="scss">
.main-screen {
  display: flex;
  justify-content: space-between;
  padding-top: 40px;
  padding-left: 40px;
  background: #292E36;
  color: white;

  @media screen and (max-width: 1085px) {
    flex-wrap: wrap;
    justify-content: center;
  }

  @media screen and (max-width: 414px) {
    padding-top: 10px;
    padding-left: 0;
  }

  &__info {
    margin: auto 0;

    @media screen and (max-width: 1085px) {
      margin-bottom: 32px;
      text-align: center;
    }

    & > h1 {
      font-family: Cormorant Infant;
      font-size: 100px;
      font-weight: 400;
      line-height: 110px;

      @media screen and (max-width: 414px) {
        font-size: 60px;
      }
    }

    & > p {
      margin-top: 26px;
      font-size: 20px;
      font-weight: 400;
      line-height: 30px;
    }
  }

  &__image {
    & > img {
      width: 635px;
      height: 740px;

      @media screen and (max-width: 1085px) {
        width: 100%;
      }
    }
  }
}

.btn {
  margin-top: 35px;
  padding: 20px 57px;
  height: 73px;
  color: #E1B168;
  border: 2px solid #e1b168;
}
</style>