<script></script>

<template>
  <section class="features">
    <h2 class="visually-hidden">Наши преимущества</h2>
    <ul class="features__list">
      <li>
        <img class="features__image" src="/images/features-mobile-1.jpg" width="314" height="232">
        <h3 class="features__title">The walkways of Indonesia spellbind</h3>
        <p class="features__text">Lorem ipsum dolor sit amet, conse <br> ctetur adip iscing elit.
          Fusce commodo magna et libero mollis rhoncus. </p>
        <a class="features__button button" href="#!">Learn More</a>
      </li>
      <li>
        <img class="features__image features__image--second" src="/images/features-mobile-2.jpg" width="314"
          height="224">
        <h3 class="features__title features__title--second">Perfect beaches exude relaxation and fun</h3>
        <p class="features__text features__text--second">Lorem ipsum dolor sit amet, conse <br> ctetur adip iscing elit.
          Fusce commodo magna et libero mollis rhoncus. </p>
        <a class="features__button button" href="#!">Learn More</a>
      </li>
    </ul>
  </section>
</template>

<style lang="scss">
.features {
  padding: 40px 30px 48px;
  background-image: url('/images/features-bg-mobile.jpg');
}

.features__list {
  display: flex;
  flex-direction: column;
  gap: 56px;
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
}

.features__button {
  height: 72px;
  padding: 22px 36px;
}
</style>
