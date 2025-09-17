<script></script>

<template>
  <section class="gallery">
    <h2 class="gallery__heading">Photo Gallery</h2>
    <p class="gallery__text">Lorem ipsum dolor sit amet, <br class="br-mobile">
      consectetur adipiscing elit. Phasellus dapibus
      mauris in lectus tempus, eget tincidunt.</p>

    <div class="gallery__wrap">
      <a class="gallery__img gallery__img--1" href="#!">
        <picture>
          <source srcset="/images/gallery-image-desktop-1.jpg" media="(min-width: 1920px)" width="370" height="530">
          <img src="/images/gallery-image-mobile-1.jpg" width="151" height="217" alt="Изображение природы.">
        </picture>
      </a>
      <a class="gallery__img gallery__img--2" href="#!">
        <picture>
          <source srcset="/images/gallery-image-desktop-2.jpg" media="(min-width: 1920px)" width="370" height="210">
          <img src="/images/gallery-image-mobile-2.jpg" width="151" height="86" alt="Изображение природы.">
        </picture>
      </a>
      <a class="gallery__img gallery__img--3" href="#!">
        <picture>
          <source srcset="/images/gallery-image-desktop-3.jpg" media="(min-width: 1920px)" width="370" height="210">
          <img src="/images/gallery-image-mobile-3.jpg" width="150" height="153" alt="Изображение природы.">
        </picture>
      </a>
      <a class="gallery__img gallery__img--4" href="#!">
        <picture>
          <source srcset="/images/gallery-image-desktop-4.jpg" media="(min-width: 1920px)" width="370" height="530">
          <img src="/images/gallery-image-mobile-4.jpg" width="151" height="86" alt="Изображение природы.">
        </picture>
      </a>
      <a class="gallery__img gallery__img--5" href="#!">
        <picture>
          <source srcset="/images/gallery-image-desktop-5.jpg" media="(min-width: 1920px)" width="370" height="370">
          <img src="/images/gallery-image-mobile-5.jpg" width="151" height="217" alt="Изображение природы.">
        </picture>
      </a>
      <a class="gallery__img gallery__img--6" a href="#!">
        <picture>
          <source srcset="/images/gallery-image-desktop-6.jpg" media="(min-width: 1920px)" width="370" height="370">
          <img src="/images/gallery-image-mobile-6.jpg" width="150" height="153" alt="Изображение природы.">
        </picture>
      </a>
    </div>
  </section>
</template>

<style lang="scss">
.gallery {
  padding: 35px 30px 40px;

  @media (min-width: 1920px) {
    padding: 169px 30px 251px;
  }
}

.gallery__heading {
  margin-bottom: 22px;
  font-size: 40px;
  line-height: 46px;
  font-family: "DM Sans", "Arial", sans-serif;
  font-weight: 700;
  text-align: center;
  color: #010a20;

  @media (min-width: 1920px) {
    font-size: 61px;
    line-height: 68px;
    margin-bottom: 35px;
  }
}

.gallery__text {
  margin-bottom: 33px;
  font-size: 16px;
  line-height: 24px;
  color: #6f7787;
  letter-spacing: 0.5px;
  text-align: center;
  font-family: "DM Sans", "Arial", sans-serif;

  @media (min-width: 1920px) {
    width: 470px;
    margin: 0 auto;
    margin-bottom: 69px;
  }
}

.gallery__wrap {
  display: grid;
  grid-template-columns: 151px 151px;
  grid-template-rows: 87px 118px 84px 154px;
  gap: 13px;

  @media (min-width: 1920px) {
    width: 1170px;
    margin: 0 auto;
    grid-template-columns: repeat(3, 370px);
    grid-template-rows: 210px 130px 130px 210px;
    gap: 30px;
    justify-content: center;
  }
}

.gallery__img {
  &--1 {
    grid-column: 1 / 2;
    grid-row: 1 / 3;
  }

  &--2 {
    grid-row: 3 / 4;
    grid-column: 1 / 2;
  }

  &--3 {
    grid-row: 4 / -1;
    grid-column: 1 / 2;
  }

  &--4 {
    grid-column: 2/-1;
    grid-row: 1 / 2;
  }

  &--6 {
    grid-row: 4 / -1;
    grid-column: 2 / -1;
  }

  @media (min-width: 1920px) {

    &--1,
    &--2,
    &--3,
    &--4,
    &--5,
    &--6 {
      grid-column: auto;
      grid-row: auto
    }

    &--3 {
      grid-row: 4;
    }

    &--4 {
      grid-column: 2;
    }

    &--5 {
      grid-column: 3 /-1;
      grid-row: 1/ 3;
    }

    &--6 {
      grid-column: 3 / -1;
      grid-row: 3 / -1;
    }
  }
}
</style>
