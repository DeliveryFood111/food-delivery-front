<template>
  <div
    class="modal fade"
    id="CartModalToggle"
    aria-labelledby="CartModalToggleLabel"
    tabindex="-1"
    aria-hidden="true"
    style="display: none"
  >
    <div class="modal-dialog modal-dialog-centered">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="CartModalToggleLabel">Замовлення</h5>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <p>
            {{ currentCart.breakfast }}
          </p>
          <p>
            {{ currentCart.first_course }}
          </p>
          <p>
            {{ currentCart.garnish }}
          </p>
          <p>
            {{ currentCart.meat }}
          </p>
          <p>
            {{ currentCart.drink }}
          </p>
        </div>
        <div class="modal-footer">
          <p>Загальна сума: {{ currentCart.price || 0 }} грн</p>
          <button type="button" class="btn btn-warning" @click="postCart">
            Підтвердити
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "Cart",
  props: {
    currentCart: Object,
  },

  methods: {
    async postCart () {
      await axios.post("https://smachno-yak-vdoma-api.herokuapp.com/cart/", this.currentCart)
        .then(function (response) {
          console.log(response);
        })
        .catch(function (error) {
          console.log(error);
        });
    },
  },
};
</script>

<style scoped lang="scss">
.modal-footer {
  justify-content: space-between;
}
</style>
