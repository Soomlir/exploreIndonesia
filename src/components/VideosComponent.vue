<script></script>

<template>
  <section class="videos">
    <h2 class="visually-hidden">Наши видео.</h2>
    <p class="videos__description">Live a life like you wouldn't imagine, experience a life you<br> wouldn't<br> expect.
    </p>
    <div class="videos__video">
      <a class="videos__img-link" href="#!">
        <img class="videos__picture" src="/images/videos-video-1-mobile.jpg" width="314" height="192"
          alt="Обложка видео.">
      </a>
    </div>
    <ul class="videos__list">
      <li class="videos__item">
        <img class="videos__image" src="/images/videos-item-1-mobile.jpg" width="314" height="176" alt="Обложка видео.">
        <h3 class="videos__heading">In The Country</h3>
        <p class="videos__text">Lorem ipsum dolor sit amet,
          consectetur adipiscing elit. Phasellus dapibus mauris in
          lectus tempus.</p>
      </li>
      <li class="videos__item">
        <img class="videos__image videos__image--second" src="/images/videos-item-2-mobile.jpg" width="314" height="176"
          alt="Обложка видео.">
        <h3 class="videos__heading videos__heading--second">In The City</h3>
        <p class="videos__text">Lorem ipsum dolor sit amet,
          consectetur adipiscing elit. Phasellus dapibus mauris in.</p>
      </li>
    </ul>
  </section>
</template>

<style lang="scss">
.videos {
  padding: 86px 30px 36px;
  background-image: url("/images/videos-bg-mobile.jpg");
}

.videos__description {
  margin-bottom: 67px;
  font-family: "DM Sans", "Arial", sans-serif;
  font-size: 40px;
  line-height: 46px;
  font-weight: 700;
  color: #ffffff;
  text-align: center;
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
}

.videos__picture {
  border-radius: 10px;
}

.videos__list {
  display: flex;
  flex-direction: column;
  gap: 34px;
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
}

.videos__image {
  margin-bottom: 34px;
  border-radius: 10px;

  &--second {
    margin-bottom: 27px;
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
}

.videos__text {
  font-size: 17px;
  line-height: 24px;
  font-family: "DM Sans", "Arial", sans-serif;
  color: rgba(255, 255, 255, 0.7);
  text-align: center;
}
</style>