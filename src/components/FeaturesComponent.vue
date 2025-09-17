<script></script>

<template>
  <section class="features">
    <h2 class="visually-hidden">Наши преимущества</h2>
    <ul class="features__list">
      <li class="features__item">
        <picture>
          <source srcset="/images/features-desktop-1.jpg" media="(min-width: 1900px)" width="630" height="460">
          <img class="features__image" src="/images/features-mobile-1.jpg" width="314" height="232">
        </picture>
        <div class="features__item-wrap">
          <h3 class="features__title">The walkways of Indonesia spellbind</h3>
          <p class="features__text">Lorem ipsum dolor sit amet, conse<br class="br-mobile">ctetur adip iscing elit.
            Fusce commodo magna et libero mollis rhoncus. </p>
          <a class="features__button button" href="#!">Learn More</a>
        </div>
      </li>
      <li class="features__item">
        <picture>
          <source srcset="/images/features-desktop-2.jpg" media="(min-width: 1900px)" width="630" height="460">
          <img class="features__image features__image--second" src="/images/features-mobile-2.jpg" width="314"
            height="224">
        </picture>
        <div class="features__item-wrap features__item-wrap--second">
          <h3 class="features__title features__title--second">Perfect beaches exude relaxation and fun</h3>
          <p class="features__text features__text--second">Lorem ipsum dolor sit amet, conse<br class="br-mobile">ctetur
            adip iscing
            elit.
            Fusce commodo magna et libero mollis rhoncus. </p>
          <a class="features__button button" href="#!">Learn More</a>
        </div>
      </li>
    </ul>
  </section>
</template>

<style lang="scss">
.features {
  padding: 40px 30px 48px;
  background-image: url('../images/features-bg-mobile.jpg');

  @media (min-width: 1920px) {
    padding: 207px 300px 267px 340px;
    background-image: url('../images/features-bg-desktop.jpg');
  }
}

.features__list {
  display: flex;
  flex-direction: column;
  gap: 56px;

  @media (min-width: 1920px) {
    gap: 159px;
  }
}

.features__item {
  @media (min-width: 1920px) {
    display: flex;
    gap: 130px;

    &:nth-child(2) {
      flex-direction: row-reverse;
    }
  }
}

.features__item-wrap {
  display: contents;

  @media (min-width: 1920px) {
    display: block;
    width: 480px;
    padding-top: 58px;

    &--second {
      padding-top: 69px;
    }
  }
}

.features__image {
  margin-bottom: 29px;
  border-radius: 10px;

  &--second {
    margin-bottom: 34px;
  }
}

.features__title {
  width: 300px;
  margin-bottom: 21px;
  font-size: 40px;
  line-height: 46px;
  font-family: "DM Sans", "Arial", sans-serif;
  color: #ffffff;

  &--second {
    margin-bottom: 26px;
  }

  @media (min-width: 1920px) {
    width: auto;
    font-size: 42px;
    line-height: 49px
  }
}

.features__text {
  margin-bottom: 31px;
  font-size: 17px;
  line-height: 24px;
  font-family: "DM Sans", "Arial", sans-serif;
  color: #e0e0e0;

  &--second {
    margin-bottom: 22px;
  }

  @media (min-width: 1920px) {
    margin-bottom: 73px;
  }
}

.br-mobile {
  display: block;

  @media (min-width: 1920px) {
    display: none;
  }
}

.features__button {
  height: 72px;
  padding: 22px 36px;

  @media (min-width: 1920px) {
    margin: 0;
    width: 180px;
    height: 59px;
    padding: 17px 36px;
  }
}
</style>
