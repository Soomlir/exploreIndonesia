<script></script>

<template>
  <section class="gallery">
    <h2 class="gallery__heading">Photo Gallery</h2>
    <p class="gallery__text">Lorem ipsum dolor sit amet, <br>
      consectetur adipiscing elit. Phasellus dapibus
      mauris in lectus tempus, eget tincidunt.</p>

    <div class="gallery__wrap">
      <a class="gallery__img gallery__img--1" href="#!">
        <img src="/images/gallery-image-mobile-1.jpg" width="151" height="217" alt="Изображение природы.">
      </a>
      <a class="gallery__img gallery__img--2" href="#!">
        <img src="/images/gallery-image-mobile-2.jpg" width="151" height="86" alt="Изображение природы.">
      </a>
      <a class="gallery__img gallery__img--3" href="#!">
        <img src="/images/gallery-image-mobile-3.jpg" width="150" height="153" alt="Изображение природы.">
      </a>
      <a class="gallery__img gallery__img--4" href="#!">
        <img src="/images/gallery-image-mobile-4.jpg" width="151" height="86" alt="Изображение природы.">
      </a>
      <a class="gallery__img gallery__img--5" href="#!">
        <img src="/images/gallery-image-mobile-5.jpg" width="151" height="217" alt="Изображение природы.">
      </a>
      <a class="gallery__img gallery__img--6" a href="#!">
        <img src="/images/gallery-image-mobile-6.jpg" width="150" height="153" alt="Изображение природы.">
      </a>
    </div>
  </section>
</template>

<style lang="scss">
.gallery {
  padding: 35px 30px 40px;
}

.gallery__heading {
  margin-bottom: 22px;
  font-size: 40px;
  line-height: 46px;
  font-family: "DM Sans", "Arial", sans-serif;
  font-weight: 700;
  text-align: center;
  color: #010a20;
}

.gallery__text {
  margin-bottom: 33px;
  font-size: 16px;
  line-height: 24px;
  color: #6f7787;
  letter-spacing: 0.5px;
  text-align: center;
  font-family: "DM Sans", "Arial", sans-serif;
}

.gallery__wrap {
  display: grid;
  grid-template-columns: 151px 151px;
  grid-template-rows: 87px 118px 84px 154px;
  gap: 13px;
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
}
</style>