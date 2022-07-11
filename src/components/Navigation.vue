<template>
  <nav class="navbar navbar-expand-lg">
    <div class="container-fluid">
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" @click="scrollToElement('benefitsEnd')">
              Чому нас обирають
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" @click="scrollToElement('benefitsEnd')">
              Наше меню
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" @click="scrollToElement('history-images')">
              Історія
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" @click="scrollToElement('history-images')">
              Спеціальні пропозиції
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" @click="scrollToElement('history-images')">
              Популярне
            </a>
          </li>
        </ul>

        <ul class="navbar-nav">
          <li class="navigation__social-links">
            <a href="https://www.instagram.com/" target="_blank">
              <img class="img" src="../assets/instagram.svg">
            </a>
          </li>
          <li class="navigation__social-links">
            <a href="https://www.facebook.com/" target="_blank">
              <img class="img" src="../assets/facebook.svg">
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navigation",
  methods: {
    scrollToElement (element) {
      const targetElement = document.querySelector(`.${element}`);
      targetElement.scrollIntoView({block: 'start', behavior: 'smooth'});
    }
  }
};
</script>

<style scoped lang="scss">
.navbar {
  padding: 26px 50px 26px 41px;
  border-top: 1px solid #5c6168;
}

.navbar-collapse {
  justify-content: space-between;
}

.navbar-nav {
  &:last-child {
    @media screen and (max-width: 993px) {
      flex-direction: row;
      margin-top: 24px;
    }
  }
}

.nav-item {
  @media screen and (max-width: 993px) {
    margin-bottom: 8px;
  }

  &:first-child {
    @media screen and (max-width: 993px) {
      margin-top: 20px;
    }
  }
}

.navbar-expand-lg .navbar-nav .nav-link {
  padding: unset;
}

.nav-link {
  margin-right: 60px;
  padding: unset;
  font-family: "Source Sans Pro";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 30px;
  color: #ffffff;

  &:hover {
    cursor: pointer;
    color: #e1b168;
  }

  @media screen and (max-width: 1192px) {
    margin-right: 20px;
  }
}

.navigation__social-links {
  margin-right: 20px;
}

.navbar-toggler {
  background: #e1b168;
}
</style>
