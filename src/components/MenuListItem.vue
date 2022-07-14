<template>
  <li class="menu__menu-list-item">
    <img src="../assets/complex-dinner.jpeg" class="menu__menu-list-item_image" />
    <div class="menu__menu-list-item_info">
      <h4>{{ title }}</h4>
      <p>{{ description }}</p>
    </div>
    <div class="menu__menu-list-item_buttons">
      <button
        class="btn btn-light menu__menu-list-item_buttons-btn"
        @click="changeCounter('-')"
      >
        <img src="../assets/minus-icon.svg" />
      </button>
      <span class="menu__menu-list-item_buttons-counter">
        {{ counter }}
      </span>
      <button
        class="btn btn-light menu__menu-list-item_buttons-btn"
        @click="changeCounter('+')"
      >
        <img src="../assets/plus-icon.svg" />
      </button>
    </div>
    <span class="menu__menu-list-item_price">{{ price }} грн</span>
  </li>
</template>

<script>
export default {
  name: "MenuListItem",
  props: {
    title: String,
    description: String,
    price: Number,
    groupIndex: Number,
  },

  data () {
    return {
      counter: 0,
      cartData: {
        title: null,
        counter: 0,
        price: 0,
        groupIndex: this.groupIndex
      }
    }
  },

  methods: {
    changeCounter (operand) {
      switch (operand) {
        case '-':
          this.counter === 0 ? this.counter : this.counter--
          this.cartData.title = this.title
          this.cartData.counter = this.counter
          this.cartData.price = this.price * this.counter

          this.$emit('addToCart', this.cartData)
          break

        case '+':
          this.counter++
          this.cartData.title = this.title
          this.cartData.counter = this.counter
          this.cartData.price = this.price * this.counter

          this.$emit('addToCart', this.cartData)
          break
      }
    }
  }
};
</script>

<style scoped lang="scss">
.menu__menu-list-item {
  display: flex;
  margin-bottom: 50px;
  min-width: 700px;

  &_image {
    margin-right: 20px;
    width: 84px;
    height: 84px;
    border-radius: 50%;
  }

  &_buttons {
    margin: auto 40px auto 0;

    &-btn {
      margin-top: unset !important;
      padding: unset !important;
      height: unset !important;
      background: unset;
      color: #E1B168;
      border: 2px solid #e1b168;
    }

    &-counter {
      margin-left: 5px;
      margin-right: 5px;
      font-size: 30px;
      font-weight: 400;
      line-height: 42px;
    }
  }

  &_info {
    margin: auto 40px auto 0;
    min-width: 357px;

    & > h4 {
      font-size: 30px;
      font-weight: 400;
      line-height: 42px;
    }

    & > p {
      margin-bottom: unset;
      font-size: 20px;
      font-weight: 400;
      line-height: 30px;
    }
  }

  &_price {
    margin: auto 0 auto 10px;
    font-size: 30px;
    font-weight: 400;
    line-height: 42px;
  }
}
</style>