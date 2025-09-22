<script></script>

<template>
  <section class="promo">
    <h1 class="promo__heading">explore <br class="promo__desktop"> indonesia</h1>
    <a class="promo__button button" href="#!">Start travelling</a>
    <div class="promo_vertical">
      <p><a href="#!">Fb</a><a href="#!">In</a><a href="#!">Tw</a></p>
      <div class="promo__progress-wrap">
        <span class="promo__number-one">01</span>
        <div class="promo__progress">
          <div></div>
        </div>
      </div>
    </div>
    <div class="promo__wrap">
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
        <img class="promo__video-img" src="/images/promo-video-bg-mobile.jpg" width="314" height="191"
          alt="Бекграунд видео.">
      </a>
    </div>
  </section>
</template>

<style lang="scss">
.promo {
  padding: 17px 0 38px 30px;

  @media (min-width: 1440px) {
    padding-top: 121px;
    padding-left: 276px;
    padding-bottom: 0;
    position: relative;
  }
}

.promo__heading {
  margin-bottom: 10px;
  font-size: 58px;
  line-height: 61px;
  font-weight: 900;
  text-transform: uppercase;
  color: #ffffff;

  @media (min-width: 1440px) {
    margin-bottom: 25px;
    font-size: 80px;
    line-height: 90px;
    font-weight: 900;
  }

  @media (min-width: 1920px) {
    margin-bottom: 25px;
    font-size: 120px;
    line-height: 130px;
    font-weight: 900;
  }
}

.promo__desktop {
  display: none;

  @media (min-width: 1440px) {
    display: block;
  }
}

.promo__button {
  margin-left: 0;
  margin-bottom: 54px;

  @media (min-width: 1440px) {
    margin: 0;
    width: 271px;
    height: 82px;
    margin-bottom: 197px;
    font-size: 20px;
    line-height: 24px;
    padding: 29px 44px;
    border-radius: 41px;
  }
}

.promo_vertical {
  display: none;

  @media (min-width: 1440px) {
    display: flex;
    position: absolute;
    transform: rotate(-90deg);
    top: 492px;

    left: -242px;

    a {
      padding: 0 20px;
      text-decoration: none;
      font-size: 16px;
      line-height: 24px;
      color: #ffffff;
    }
  }

  @media (min-width: 1920px) {
    left: -339px;
  }
}

.promo__progress-wrap {
  @media (min-width: 1440px) {
    display: flex;
    gap: 20px;
    align-items: center;
    margin-left: 86px;
  }

  @media (min-width: 1920px) {
    margin-left: 215px;
  }
}

.promo__number-one {
  font-family: "DM Sans", "Arial", sans-serif;
  font-size: 16px;
  line-height: 24px;
  font-weight: 700;
  color: #ffffff;
}

.promo__progress {
  width: 396px;
  height: 2px;
  background-color: #ffffff;
  display: flex;

  div {
    margin-left: auto;
    width: 100px;
    height: 4px;
    background-color: #dd2242;
  }
}

.promo__wrap {
  display: contents;

  @media (min-width: 1440px) {
    display: flex;
  }
}

.promo__list {
  display: flex;
  flex-direction: column;
  width: 315px;
  gap: 58px;
  padding: 59px 33px 31px;
  background-color: rgba(0, 0, 0, 0.6);
  counter-reset: my-counter;
  box-sizing: border-box;

  @media (min-width: 1440px) {
    flex-direction: row;
    gap: 127px;
    width: 946px;
    height: 210px;
    margin-top: 44px;
    padding-left: 71px;
    padding-top: 75px;
    box-sizing: border-box;
  }

  @media (min-width: 1920px) {
    flex-direction: row;
    gap: 200px;
    width: 1226px;
    height: 210px;
    margin-top: 44px;
    padding-left: 71px;
    padding-top: 75px;
    box-sizing: border-box;
  }
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

  @media (min-width: 1920px) {
    &:before {
      top: -33px;
    }
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

  @media (min-width: 1920px) {
    width: 209px;
    font-size: 19px;
    line-height: 27px;
  }
}

.promo__video {
  position: relative;
  display: flex;
  width: 315px;

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
    background-image: url('../images/play.svg');
  }

  @media (min-width: 1920px) {
    width: 418px;

    &::before {
      width: 78px;
      height: 78px;
    }
  }
}

.promo__video-img {
  @media (min-width: 1920px) {
    width: 418px;
    height: 254px;
  }
}
</style>
