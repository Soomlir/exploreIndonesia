<script></script>

<template>
  <section class="videos">
    <h2 class="visually-hidden">Наши видео.</h2>
    <p class="videos__description">Live a life like you wouldn't imagine, experience a life you<br class="br-mobile">
      wouldn't<br class="br-mobile"> expect.
    </p>
    <div class="videos__video">
      <a class="videos__img-link" href="#!">
        <picture>
          <source srcset="/images/videos-video-1-desktop.jpg" media="(min-width: 1920px)" width="1056" height="594">
          <img class="videos__picture" src="/images/videos-video-1-mobile.jpg" width="314" height="192"
            alt="Обложка видео.">
        </picture>
      </a>
    </div>
    <ul class="videos__list">
      <li class="videos__item">
        <img class="videos__image" src="/images/videos-item-1-mobile.jpg" width="314" height="176" alt="Обложка видео.">
        <div class="videos__item-wrap">
          <h3 class="videos__heading">In The Country</h3>
          <p class="videos__text">Lorem ipsum dolor sit amet,
            consectetur adipiscing elit. Phasellus dapibus mauris in
            lectus tempus.</p>
        </div>
      </li>
      <li class="videos__item">
        <img class="videos__image videos__image--second" src="/images/videos-item-2-mobile.jpg" width="314" height="176"
          alt="Обложка видео.">
        <div class="videos__item-wrap">
          <h3 class="videos__heading videos__heading--second">In The City</h3>
          <p class="videos__text">Lorem ipsum dolor sit amet,
            consectetur adipiscing elit. Phasellus dapibus mauris in.</p>
        </div>
      </li>
    </ul>
  </section>
</template>

<style lang="scss">
.videos {
  padding: 86px 30px 36px;
  background-image: url("/images/videos-bg-mobile.jpg");

  @media (min-width: 1920px) {
    padding: 146px 30px 221px;
    background-image: url("/images/videos-bg-desktop.jpg");
  }
}

.videos__description {
  margin-bottom: 67px;
  font-family: "DM Sans", "Arial", sans-serif;
  font-size: 40px;
  line-height: 46px;
  font-weight: 700;
  color: #ffffff;
  text-align: center;

  @media (min-width: 1920px) {
    width: 1007px;
    margin: 0 auto;
    margin-bottom: 113px;
  }
}

.videos__video {
  margin-bottom: 40px;
}

.videos__img-link {
  display: flex;
  position: relative;

  &::before {
    content: "";
    position: absolute;
    inset: 0;
    margin: auto;
    width: 67px;
    height: 67px;
    background-color: #e93a7d;
    border-radius: 50%;
  }


  &::after {
    position: absolute;
    content: "";
    width: 16px;
    height: 16px;
    inset: 0;
    margin: auto;
    background-image: url("/images/play-white.svg");
    background-repeat: no-repeat;
  }

  @media (min-width: 1920px) {
    width: 1056px;
    margin: 0 auto;

    &::before {
      width: 96px;
      height: 96px;
    }
  }
}

.videos__picture {
  border-radius: 10px;
}

.videos__list {
  display: flex;
  flex-direction: column;
  gap: 34px;

  @media (min-width: 1920px) {
    flex-direction: row;
    gap: 64px;
    width: 1223px;
    margin: 0 auto;
    margin-top: 120px;
  }
}

.videos__item-wrap {
  display: contents;

  @media (min-width: 1920px) {
    display: block;
  }
}

.videos__item {
  position: relative;

  &::before {
    content: "";
    position: absolute;
    width: 16px;
    height: 16px;
    top: 79px;
    left: 152px;
    background-image: url("/images/play-white.svg");
  }

  @media (min-width: 1920px) {
    display: flex;
    gap: 42px;

    &::before {
      top: 62px;
      left: 107px;
    }
  }
}

.videos__image {
  margin-bottom: 34px;
  border-radius: 10px;

  &--second {
    margin-bottom: 27px;
  }

  @media (min-width: 1920px) {
    width: 233px;
    height: 151px;
  }
}

.videos__heading {
  margin-bottom: 21px;
  font-size: 22px;
  line-height: 150%;
  text-align: center;
  color: #ffffff;
  font-family: "DM Sans", "Arial", sans-serif;

  &--second {
    margin-bottom: 19px;
  }

  @media (min-width: 1920px) {
    text-align: left;
  }
}

.videos__text {
  font-size: 17px;
  line-height: 24px;
  font-family: "DM Sans", "Arial", sans-serif;
  color: rgba(255, 255, 255, 0.7);
  text-align: center;

  @media (min-width: 1920px) {
    text-align: left;
  }
}
</style>