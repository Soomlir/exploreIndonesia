<script></script>

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
body {
	margin: 0;
	font-family: "Roboto", "Arial", sans-serif;
	font-size: 13px;
	line-height: 20px;
	font-weight: 400;
}

.visually-hidden {
	position: fixed;
	transform: scale(0);
}

ul {
	margin: 0;
	padding: 0;
	list-style: none;
}

h1,
h2,
h3 {
	margin: 0;
}

p {
	margin: 0;
}

.header {
  display: flex;
  padding: 48px 0 15px;
}

.header__gamburger {
  span {
    display: block;
    width: 18px;
    height: 2px;
    background-color: #ffffff;
  }
}
</style>
