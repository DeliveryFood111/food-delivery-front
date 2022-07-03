<template>
  <footer class="footer">
    <div class="footer__top">
      <div class="footer__top-contacts">
        <p class="footer__top-contacts-hashtag">#FoodDelivery</p>
        <div class="footer__top-contacts-info">
          <h6 class="footer__top-contacts-info-title">Контакты</h6>
          <p class="footer__top-contacts-info-item">22 Радужная, Киев</p>
          <p class="footer__top-contacts-info-item">+123 456 789</p>
          <p class="footer__top-contacts-info-item">josefin@mail.com</p>
        </div>
      </div>
      <div class="footer__top-logo-with-button">
        <img class="img" src="../assets/product-logo.svg" />
        <p class="footer__top-logo-with-button-info">
          Заказывайте доставку еды, узнайте историю любимой кухни, следите за
          нами в социальных сетях, живите в своё удовольствие!
        </p>
      </div>
      <div class="footer__top-social-links-with-worktime">
        <ul class="footer__top-social-links-with-worktime_social-links">
          <li>
            <a href="https://www.instagram.com/" target="_blank">
              <img class="img" src="../assets/instagram.svg" />
            </a>
          </li>
          <li>
            <a href="https://www.facebook.com/" target="_blank">
              <img class="img" src="../assets/facebook.svg" />
            </a>
          </li>
          <li>
            <a href="https://twitter.com/" target="_blank">
              <img class="img" src="../assets/twitter.svg" />
            </a>
          </li>
          <li>
            <a href="https://stackoverflow.com/" target="_blank">
              <img class="img" src="../assets/stackoverflow.svg" />
            </a>
          </li>
        </ul>
        <div class="footer__top-social-links-with-worktime_worktime">
          <h6 class="footer__top-social-links-with-worktime-title">
            Часы работы
          </h6>
          <p class="footer__top-social-links-with-worktime-time">
            <span>Пон – Пят: </span>7.00 – 20.00
          </p>
          <p class="footer__top-social-links-with-worktime-time">
            <span>Суб: </span>7.00 – 20.00
          </p>
          <p class="footer__top-social-links-with-worktime-time">
            <span>Вос: </span>8.00 - 20.00
          </p>
        </div>
      </div>
    </div>
    <div class="footer__bottom">© Copyright - TastEat | Created by Me</div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
.footer {
  width: 100%;
  background: #292e36;
  color: white;

  &__top {
    display: flex;
    justify-content: space-between;
    padding: 130px 24px 40px;

    &-contacts {
      &-hashtag {
        font-size: 22px;
        font-weight: 400;
        line-height: 33px;
      }

      &-info {
        margin-top: 132px;

        &-title {
          width: fit-content;
          margin-bottom: 32px;
          border-top: 1px solid #e1b168;
          border-bottom: 1px solid #e1b168;
        }

        &-item {
          margin-bottom: unset;
          font-size: 20px;
          font-weight: 400;
          line-height: 30px;
          color: #e1b168;
        }
      }
    }

    &-logo-with-button {
      justify-content: center;
      display: flex;
      flex-direction: column;
      max-width: 303px;
      text-align: center;

      @media screen and (max-width: 680px) {
        display: none;
      }

      &-info {
        margin-top: 32px;
        font-size: 20px;
        font-weight: 400;
        line-height: 30px;
      }
    }

    &-social-links-with-worktime {
      &_social-links {
        padding-left: unset;
        margin-bottom: 62px;
        list-style: none;

        & > li {
          width: fit-content;

          &:first-child {
            margin-left: auto;
          }

          &:nth-child(3n) {
            margin-left: 30%;
          }

          &:last-child {
            margin-left: 60%;
          }
        }
      }

      &_worktime {
        text-align: end;
      }

      &-title {
        margin-left: auto;
        margin-bottom: 32px;
        width: fit-content;
        border-top: 1px solid #e1b168;
        border-bottom: 1px solid #e1b168;
      }

      &-time {
        margin-bottom: 5px;

        & > span {
          color: #E1B168;
        }
      }
    }
  }

  &__bottom {
    padding: 18px 25px;
    border-top: 1px solid #575b62;
  }
}
</style>
