<template>
  <header class="header">
    <div class="header__top">
      <a href="tel: +380667916850">
        <button class="btn btn-dark" type="button">
          Подзвонити +38(066) 791 68 50
        </button>
      </a>
      <img class="img" src="../assets/product-logo.svg">
      <a class="btn btn-warning" data-bs-toggle="modal" href="#CartModalToggle" role="button">
        <p class="btn_text">
          Кошик
          <img  class="btn_icon" src="../assets/basket-icon.svg">
        </p>
      </a>
    </div>
    <Navigation />
  </header>
</template>

<script>
import Navigation from "@/components/Navigation";

export default {
  name: "Header",
  components: { Navigation },
};
</script>

<style scoped lang="scss">
.header {
  background: #292e36;

  &__top {
    display: flex;
    justify-content: space-between;
    padding: 50px 40px;

    @media screen and (max-width: 993px) {
      display: none;
    }
  }
}

.btn {
  margin-top: auto;
  margin-bottom: auto;
  padding: 20px 57px;
  height: 73px;
  border: 2px solid #e1b168;

  &_text {
    margin: auto 0;
  }

  &_icon {
    margin-left: 5px;
  }
}

a {
  margin-top: auto;
  margin-bottom: auto;
  height: 100%;
}
</style>
