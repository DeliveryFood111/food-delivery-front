<template>
  <header class="header">
    <div class="header__top">
      <a href="tel: 123456789">
        <button class="btn btn-dark" type="button">
          Позвонить - 123 456 789
        </button>
      </a>
      <img class="img" src="../assets/product-logo.svg">
      <button class="btn btn-warning" type="button">Перейти к заказу</button>
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
}

a {
  margin-top: auto;
  margin-bottom: auto;
  height: 100%;
}
</style>
