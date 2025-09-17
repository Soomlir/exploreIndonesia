<script setup></script>

<template>
  <header class="header">
    <a class="header__logo" href="#!">
      <img class="header__logo-img" src="/images/logo.svg" alt="Лого сайта.">
    </a>
    <ul class="header__menu">
      <li class="header__item">
        <a href="#!" class="header__link">Destinations</a>
      </li>
      <li class="header__item">
        <a href="#!" class="header__link">Experiences</a>
      </li>
      <li class="header__item">
        <a href="#!" class="header__link">About</a>
      </li>
      <li class="header__item">
        <a href="#!" class="header__link">Gallery</a>
      </li>
    </ul>
    <a class="header__search" href="#!">
      <span class="visually-hidden">Поиск.</span>
    </a>
    <div class="header__gamburger">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </header>
</template>

<style lang="scss">
.header {
  display: flex;
  padding: 48px 34px 24px 24px;

  @media (min-width: 1920px) {
    padding: 28px 145px 39px 20px;
  }
}

.header__logo {
  margin-right: auto;

  @media (min-width: 1920px) {
    margin: 0;
    margin-right: 42px;
  }
}

.header__logo-img {
  width: 149px;

  @media (min-width: 1920px) {
    width: 185px;
    height: 68px;
  }
}

.header__menu {
  display: none;

  @media (min-width: 1920px) {
    display: flex;
    align-items: center;
    margin-right: auto;
  }
}

.header__link {
  display: block;
  padding: 22px 30px;
  text-decoration: none;
  font-size: 18px;
  line-height: 24px;
  color: #ffffff;
  font-family: "DM Sans", "Arial", sans-serif;
  font-weight: 700;
  text-transform: uppercase;
}

.header__search {
  display: block;
  width: 20px;
  height: 20px;
  margin-top: 10px;
  margin-right: 36px;
  background-image: url('../images/search.svg');

  @media (min-width: 1920px) {
    margin-top: 15px;
  }
}

.header__gamburger {
  margin-top: 14px;
  cursor: pointer;

  span {
    display: block;
    width: 18px;
    height: 2px;
    margin-bottom: 3px;
    background-color: #ffffff;
  }

  @media (min-width: 1920px) {
    display: none;
  }
}
</style>
