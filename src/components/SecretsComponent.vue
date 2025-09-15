<script></script>

<template>
  <section class="secrets">
    <h2 class="secrets__heading">Explore Our Secrets</h2>
    <div class="secrets__slider-wrap">
      <ul class="secrets__slider slider">
        <li class="slider__item">
          <img class="slider__image" src="/images/slide-mobile-1.jpg" width="314" height="200" alt="Слайд первый.">
        </li>
        <div class="slider__controls">
          <button class="slider__button-control">
            <span class="visually-hidden">Кнопка переключения слайда.</span>
          </button>
          <button class="slider__button-control">
            <span class="visually-hidden">Кнопка переключения слайда.</span>
          </button>
          <button class="slider__button-control">
            <span class="visually-hidden">Кнопка переключения слайда.</span>
          </button>
          <button class="slider__button-control slider__button-control--current">
            <span class="visually-hidden">Кнопка переключения слайда.</span>
          </button>
          <button class="slider__button-control">
            <span class="visually-hidden">Кнопка переключения слайда.</span>
          </button>
        </div>
        <button class="slider__prev">
          <span class="visually-hidden">Предыдущий слайд.</span>
        </button>
        <button class="slider__next">
          <span class="visually-hidden">Следующий слайд.</span>
        </button>
      </ul>
    </div>
  </section>
</template>
<style lang="scss">
.secrets {
  padding-top: 35px;
  background-image: url("/images/secrets-bg-mobile.jpg");
}

.secrets__heading {
  margin-bottom: 33px;
  font-size: 40px;
  line-height: 46px;
  font-family: "DM Sans", "Arial", sans-serif;
  color: #010a20;
  text-align: center;
}

.secrets__slider-wrap {
  position: relative;
  padding-bottom: 700px;
}

.slider__prev,
.slider__next {
  position: absolute;
  width: 12px;
  height: 20px;
  border: none;
  background: none;
  background-image: url('/images/arrow-left-mobile.svg');
  cursor: pointer;
}

.slider__prev {
  top: 91px;
  left: 7px;
}

.slider__next {
  top: 91px;
  right: 10px;
  transform: scale(-1);
}

.slider__image {
  display: block;
  margin: 0 auto;
  border-radius: 10px;
}

.slider__controls {
  width: 182px;
  margin: 0 auto;
  margin-top: 16px;
}

.slider__button-control {
  width: 17px;
  height: 17px;
  margin: 0 7px;
  border: none;
  border-radius: 50%;
  background-color: #85a3b2;
  cursor: pointer;

  &--current {
    width: 44px;
    background-color: #dd2242;
    border-radius: 60px;
  }
}
</style>
