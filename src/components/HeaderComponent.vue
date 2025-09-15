<script setup></script>

<template>
  <header class="header">
    <a class="header__logo" href="#!">
      <img src="/images/logo.svg" alt="Лого сайта.">
    </a>
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
}

.header__logo {
  margin-right: auto;
}

.header__search {
  display: block;
  width: 20px;
  height: 20px;
  margin-top: 10px;
  margin-right: 36px;
  background-image: url('/images/search.svg');
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
}
</style>
