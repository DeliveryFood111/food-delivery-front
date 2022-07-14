<template>
  <section class="menu">
    <div class="menu__about">
      <h2 class="menu__about-title">Комплексне харчування</h2>
      <p class="menu__about-description">
        Основною відминністю нас від інших компаній є можливість замовлення
        комплексу страв, на весь день. Займайся своїми справами, а про
        харчування подбаємо ми!
      </p>
      <img src="../assets/complex-dinner.jpeg" class="menu__about-image" />
      <Cart :currentCart="currentCart" />
      <a
        class="btn btn-light"
        data-bs-toggle="modal"
        href="#CartModalToggle"
        role="button"
      >
        Кошик
      </a>
    </div>
    <div class="menu__menu-wrapper">
      <div
        class="menu__menu-list"
        v-for="(item, index) in menuItems"
        :key="`${item}-${index}`"
      >
        <h3 class="menu__menu-list-title">{{ item.title }}</h3>
        <ul>
          <MenuListItem
            v-for="(item, inx) in item.items"
            :key="`${item}-${inx}`"
            :title="item.title"
            :description="item.description"
            :price="item.price"
            :groupIndex="index"
            @addToCart="addToCart"
          />
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
import MenuListItem from "@/components/MenuListItem";
import Cart from "@/components/Cart";

export default {
  name: "Menu",
  components: { Cart, MenuListItem },

  data() {
    return {
      menuItems: [
        {
          title: "Сніданок",
          items: [
            {
              title: "Запеканка з вишнями",
              description: "Запеканка з вишнями",
              price: 38,
            },
            {
              title: "Сирники",
              description: "Shuck the scallop to that used for oysters",
              price: 42,
            },
            {
              title: "Бризоль",
              description: "Shuck the scallop to that used for oysters",
              price: 34,
            },
            {
              title: "Омлет з беконом і овочами",
              description: "Омлет з беконом і овочами",
              price: 49,
            },
            {
              title: "Овсянка з ягодами",
              description: "Овсянка з ягодами",
              price: 35,
            },
            {
              title: "Омлетна запеканка",
              description: "Омлетна запеканка",
              price: 44,
            },
          ],
        },
        {
          title: "Перше",
          items: [
            {
              title: "Борщ",
              description: "Традиційне українське перше блюдо",
              price: 70,
            },
            {
              title: "Гороховий суп",
              description: "Shuck the scallop to that used for oysters",
              price: 60,
            },
            {
              title: "Суп з фрикадельками",
              description: "Shuck the scallop to that used for oysters",
              price: 65,
            },
            {
              title: "Харчо",
              description: "Shuck the scallop to that used for oysters",
              price: 63,
            },
          ],
        },
        {
          title: "Гарнір",
          items: [
            {
              title: "Гречка",
              description: "Гречана каша",
              price: 44,
            },
            {
              title: "Макарони",
              description: "Shuck the scallop to that used for oysters",
              price: 39,
            },
            {
              title: "Паста (Баланьєз)",
              description: "Shuck the scallop to that used for oysters",
              price: 70,
            },
            {
              title: "Картопля пюре",
              description: "Картопля пюре",
              price: 49,
            },
            {
              title: "Картопля по-селянські",
              description: "Картопля по-селянські",
              price: 35,
            },
          ],
        },
        {
          title: "М'ясо",
          items: [
            {
              title: "Ніжка куряча, запечена",
              description: "Ніжка куряча, запечена",
              price: 38,
            },
            {
              title: "Яловичина тушена",
              description: "Shuck the scallop to that used for oysters",
              price: 42,
            },
            {
              title: 'Котлета "По-київськи"',
              description: "Shuck the scallop to that used for oysters",
              price: 77,
            },
            {
              title: "Гречаники",
              description: "Гречаники",
              price: 49,
            },
            {
              title: "Голубці",
              description: "Голубці",
              price: 65,
            },
            {
              title: "Риба смажена",
              description: "Риба смажена",
              price: 44,
            },
            {
              title: "Курка з овочами",
              description: "Курка з овочами",
              price: 44,
            },
            {
              title: 'Котлета "Домашня"',
              description: 'Котлета "Домашня"',
              price: 44,
            },
          ],
        },
        {
          title: "Напій",
          items: [
            {
              title: "Компот",
              description: "Компот домашній",
              price: 18,
            },
            {
              title: "Coca-cola",
              description: "Shuck the scallop to that used for oysters",
              price: 22,
            },
            {
              title: "Мінеральна вода",
              description: "Shuck the scallop to that used for oysters",
              price: 34,
            },
            {
              title: "Сік",
              description: "Сік",
              price: 49,
            },
          ],
        },
      ],
      currentCart: {
        name: "Dev",
        price: null,
        breakfast: "",
        first_course: "",
        garnish: "",
        meat: "",
        drink: "",
        address: "Dev street, 007",
        phone_number: "777",
      },
      groups: ["breakfast", "first_course", "garnish", "meat", "drink"],
    };
  },

  methods: {
    addToCart({ title, counter, price, groupIndex }) {
      this.currentCart[this.groups[groupIndex]] =
        counter === 0
          ? this.currentCart[this.groups[groupIndex]]
          : this.currentCart[this.groups[groupIndex]] + `${title} x${counter} `;
      this.currentCart.price = this.currentCart.price + price;

      console.log(this.currentCart);
    },
  },
};
</script>

<style scoped lang="scss">
.menu {
  display: flex;
  justify-content: space-between;
  padding: 140px 40px;

  &__about {
    margin-right: 55px;
    max-width: 486px;

    &-title {
      font-size: 40px;
      font-weight: 400;
      line-height: 56px;
    }

    &-description {
      margin-top: 14px;
      font-size: 20px;
      font-weight: 400;
      line-height: 30px;
    }

    &-image {
      margin-top: 45px;
      width: 398px;
      height: 548px;
    }
  }

  &__menu-list {
    & > ul {
      padding-left: unset;
      list-style: none;
    }

    &-title {
      margin-bottom: 40px;
      font-size: 36px;
      font-weight: 400;
      line-height: 50px;
    }
  }
}

.btn {
  margin-top: 60px;
  padding: 20px 57px;
  height: 73px;
  background: unset;
  color: #e1b168;
  border: 2px solid #e1b168;
}
</style>
