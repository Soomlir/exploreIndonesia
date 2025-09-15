<script></script>

<template>
  <section class="promo">
    <h1 class="promo__heading">explore indonesia</h1>
    <a class="promo__button button" href="#!">Start travelling</a>
    <ol class="promo__list">
      <li class="promo__item">
        <h3 class="promo__title">Title here</h3>
        <p class="promo__text">Lorem ipsum dolor sit amet et amet ist ame.</p>
      </li>
      <li class="promo__item">
        <h3 class="promo__title">Title here</h3>
        <p class="promo__text">Lorem ipsum dolor sit amet et amet ist ame.</p>
      </li>
      <li class="promo__item">
        <h3 class="promo__title">Title here</h3>
        <p class="promo__text">Lorem ipsum dolor sit amet et amet ist ame.</p>
      </li>
    </ol>
    <a class="promo__video" href="#!">
      <img src="/images/promo-video-bg-mobile.jpg" width="314" height="191" alt="Бекграунд видео.">
    </a>
  </section>
</template>

<style lang="scss">
.promo {
  padding: 17px 30px 40px;
}

.promo__heading {
  margin-bottom: 10px;
  font-size: 58px;
  line-height: 61px;
  font-weight: 900;
  text-transform: uppercase;
  color: #ffffff;
}

.promo__button {
  margin-bottom: 54px;
}

.promo__list {
  display: flex;
  flex-direction: column;
  gap: 58px;
  padding: 59px 33px 31px;
  background-color: rgba(0, 0, 0, 0.6);

  counter-reset: my-counter;
}

.promo__item {
  position: relative;
  counter-increment: my-counter;

  &::before {
    content: counter(my-counter, decimal-leading-zero);
    position: absolute;
    top: -23px;
    left: 0;
    color: #dd2242;
    font-weight: bold;
    font-size: 1.2em;
  }
}

.promo__title {
  font-size: 26px;
  line-height: 41px;
  color: #ffffff;
  font-family: "DM Sans", "Arial", sans-serif;
}

.promo__text {
  width: 187px;
  font-size: 17px;
  line-height: 24px;
  color: #939393;
  font-family: "DM Sans", "Arial", sans-serif;
}

.promo__video {
  position: relative;
  display: flex;

  &::before {
    content: "";
    position: absolute;
    width: 58px;
    height: 59px;
    inset: 0;
    margin: auto;
    border-radius: 50%;
    background-color: #ffffff;
    box-shadow: 0 0 50px rgba(0, 0, 0, 0.5);
  }

  &::after {
    position: absolute;
    content: "";
    width: 34px;
    height: 33px;
    inset: 0;
    margin: auto;
    background-image: url('/images/play.svg');
  }
}
</style>
