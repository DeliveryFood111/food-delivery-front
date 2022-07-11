<template>
  <section class="popular-product">
    <div class="popular-product__case_content">
      <h3 class="popular-product__title">
        MENU
      </h3>
      <p class="popular-product__case_content-title">
        Popular Dishes
      </p>
      <p class="popular-product__case_content-text">
        There is a game between the waiters in restaurant to see who serves the food to each table fastest. That led to attempting the Guinness Record.
      </p>
    </div>
    <div class="popular-product__case_menu">
      <div class="popular-product__case_menu_cells" >
        <img src="../assets/ukraine-borsch.webp" class="popular-product__case_menu_cells_img">
        <div class="popular-product__case_menu_cells_price">
          <p class="popular-product__case_menu_cells_price-text">
            Chicken Manjoori
          </p>
          <p class="popular-product__case_menu_cells_price-text">
            $15
          </p>
        </div>
        <div class="popular-product__case_menu_cells_description">
          Dish relished by all age groups as a starter dish at parties.
        </div>
      </div>
      <div class="popular-product__case_menu_cells" >
        <img  src="../assets/vareniki.webp" class="popular-product__case_menu_cells_img">
        <div class="popular-product__case_menu_cells_price">
          <p class="popular-product__case_menu_cells_price-text">
            Hotdog
          </p>
          <p class="popular-product__case_menu_cells_price-text">
            $10
          </p>
        </div>
        <div class="popular-product__case_menu_cells_description">
          Grilled sausage served in the slit of a partially sliced bun.
        </div>
      </div>
      <div class="popular-product__case_menu_cells" >
        <img  src="../assets/salad.webp" class="popular-product__case_menu_cells_img">
        <div class="popular-product__case_menu_cells_price">
          <p class="popular-product__case_menu_cells_price-text">
            Fresh Salmon
          </p>
          <p class="popular-product__case_menu_cells_price-text">
            $5
          </p>
        </div>
        <div class="popular-product__case_menu_cells_description">
          Beat the health blues with our Super Immune Blue Juice Recipe.
        </div>
      </div>
      <div class="popular-product__case_menu_cells" >
        <img src="../assets/hachapuri-po-adjarski.webp" class="popular-product__case_menu_cells_img">
        <div class="popular-product__case_menu_cells_price">
          <p class="popular-product__case_menu_cells_price-text">
            Veg Burger
          </p>
          <p class="popular-product__case_menu_cells_price-text">
            $10
          </p>
        </div>
        <div class="popular-product__case_menu_cells_description">
          Burgers may be made from ingredients like beans.
        </div>
      </div>
    </div>
    <div class="popular-product__case_btn">
      <button class="popular-product__case_btn-button"> See all dishes </button>
    </div>
  </section>
</template>

<script>
export default {
  name: "PopularProducts" ,
}
</script>
<style scoped lang="scss">

.popular-product {
  color: rgba(41, 46, 54, 1);
  background-color: rgba(220, 220, 220, 1);
  display: flex;
  flex-direction: column;
  text-align: center;
  padding: 40px;

  &__title {
    border-top: 2px solid rgba(225, 177, 104, 1);
    border-bottom: 2px solid rgba(225, 177, 104, 1);
    font-size: 15px;
    font-weight: 400;
    line-height: 23px;
    letter-spacing: 3px;
    margin-bottom: 12px;
  }

  &__case_content {
    display: flex;
    flex-direction: column;
    margin-bottom: 15px;
    align-items: center;

    &-title {
      font-size: 40px;
      font-weight: 400;
      line-height: 56px;
      margin: 0 auto;
    }

    &-text {
      font-size: 20px;
      font-weight: 400;
      line-height: 30px;


    }
  }
  &__case_menu {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    margin-bottom: 30px;
    flex-wrap: wrap;

    @media screen and (max-width: 900px){
      flex-direction: column;
      align-content: center;
    }
    &_cells {
      display: flex;
      flex-direction: column;
      width: 220px;

      @media screen and (max-width: 1050px){
        margin-bottom: 30px;
        margin-left: 50px;
        width: 350px;
      }
      @media screen and (max-width: 900px){
        margin-left: unset;
      }

      @media screen and (max-width: 780px){
        align-items: center;
        width: 280px;
      }
      &_img {
        width: 220px;
        height: 250px;
        margin-bottom: 9px;

        @media screen and (max-width: 1050px){
          width: 350px;
        }
        @media screen and (max-width: 780px){
          width: 280px;
          height: 230px;
        }
      }
      &_description {
        padding-top: 10px;
        border-top: 2px solid grey;
        font-size: 20px;
        font-weight: 400;
        line-height: 30px;
      }
      &_price {
        display: flex;
        flex-direction: row;
        width: 220px;
        justify-content: space-between;
        font-size: 20px;
        margin-bottom: 15px;
        font-weight: 700;
        line-height: 42px;

        @media screen and (max-width: 1050px){
          margin-bottom: 10px;
          width: 350px;
        }
        @media screen and (max-width: 780px){
          width: 280px;
        }
        &-text {
          margin-top: 0;
          margin-bottom: 0;
        }
      }
    }
  }

  &__case_btn {

    &-button {
      border: 2px solid rgba(225, 177, 104, 1);
      color: rgba(225, 177, 104, 1);
      background-color: rgba(220, 220, 220, 1);
      padding: 20px 40px;
      height: 73px;
      width: 255px;
      font-size: large;

      &:hover {
        text-shadow: 0px 0px 2px rgba(225, 177, 104, 1);
        box-shadow: 0px 0px 5px 3px rgba(225, 177, 104, 1);
        border: 2px solid rgba(225, 177, 104, 1);
      }
    }
  }
}
</style>