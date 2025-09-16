<script></script>

<template>
  <section class="plan">
    <h2 class="visually-hidden">Наш план</h2>
    <p class="plan__description">Getting there</p>
    <ol class="plan__list">
      <li class="plan__item">
        <h3 class="plan__heading">Bookings your flights</h3>
        <p class="plan__text">Lorem ipsum dolor set,,,,<br>
          <a class="plan__link" href="#!">Show more</a>
        </p>
      </li>
      <li class="plan__item">
        <h3 class="plan__heading plan__heading--second">Choosing your hotel</h3>
        <p class="plan__text plan__text--second">Lorem ipsum dolor set,,,,<br>
          <a class="plan__link" href="#!">Show more</a>
        </p>
        <div class="plan__preview-wrap">
          <a href="#!">
            <img src="/images/plan-preview-mobile.jpg" width="314" height="208" alt="Обложка видео.">
          </a>
        </div>
        <p class="plan__text plan__text--second">Lorem ipsum dolor set,,,,<br>
          <a class="plan__link" href="#!">Show more</a>
        </p>
      </li>
      <li class="plan__item">
        <h3 class="plan__heading">Planning your experiences</h3>
        <p class="plan__text">Lorem ipsum dolor set,,,,<br>
          <a class="plan__link" href="#!">Show more</a>
        </p>
      </li>
    </ol>
  </section>
</template>

<style lang="scss">
.plan {
  padding: 30px 30px 81px;
  background-color: #dce8f2;

  @media (min-width: 1920px) {
    padding: 130px 353px 81px;
  }
}

.plan__description {
  margin-bottom: 33px;
  color: #010a20;
  font-size: 40px;
  line-height: 46px;
  font-family: "DM Sans", "Arial", sans-serif;
  font-weight: 700;
  text-align: center;

  @media (min-width: 1920px) {
    text-align: left;
    margin-left: 36px;
    font-size: 59px;
    line-height: 53px;
  }
}

.plan__list {
  counter-reset: my-counter;
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.plan__item {
  padding-top: 90px;
  position: relative;
  counter-increment: my-counter;
  display: flex;
  align-items: center;
  flex-direction: column;

  &::before {
    content: counter(my-counter);
    position: absolute;
    top: 5%;
    left: 41%;
    width: 56px;
    height: 56px;
    background-color: #dd2242;
    color: #ffffff;
    font-weight: bold;
    font-size: 1.5em;
    border-radius: 50%;
    font-size: 27px;
    line-height: 38px;
    font-family: "DM Sans", "Arial", sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    line-height: 1;
  }
}

.plan__heading {
  margin-bottom: 5px;
  font-size: 22px;
  line-height: 150%;
  font-family: "DM Sans", "Arial", sans-serif;
  color: #010a20;
  text-align: center;

  &--second {
    margin-bottom: 14px;
  }
}

.plan__text {
  font-size: 17px;
  line-height: 24px;
  font-family: "DM Sans", "Arial", sans-serif;
  color: rgba(#151439, 0.4);
  text-align: center;
  text-decoration: none;

  &--second {
    margin-bottom: 33px;
  }
}

.plan__link {
  text-decoration: none;
  font-size: 17px;
  line-height: 24px;
  font-family: "DM Sans", "Arial", sans-serif;
  color: #dd2242;
}

.plan__preview-wrap {
  margin-bottom: 38px;
  position: relative;

  &::before {
    content: "";
    position: absolute;
    width: 16px;
    height: 16px;
    inset: 0;
    margin: auto;
    background-image: url("/images/play-white.svg");
  }
}
</style>