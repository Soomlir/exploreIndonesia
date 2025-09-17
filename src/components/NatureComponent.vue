<script></script>

<template>
  <section class="nature">
    <h2 class="nature__heading">Our hills and valleys are like<br class="br-desktop"> nothing you’ve seen.</h2>
    <p class="nature__text">Lorem ipsum dolor sit amet, <br class="br-mobile"> consectetur adipiscing elit.
      Fusce sit amet magna commodo, tempus dolor sit amet,
      laoreet elit. Donec mauris tortor, elementum sed.</p>
    <a class="nature__button button" href="#!">Learn More</a>
  </section>
</template>

<style lang="scss">
.nature {
  padding: 171px 30px 116px;
  background-image: url("../images/nature-bg-mobile.jpg");

  @media (min-width: 1920px) {
    padding: 249px 30px 257px;
    background-image: url("../images/nature-bg-desktop.jpg");
  }
}

.nature__heading {
  margin-bottom: 34px;
  color: #000000;
  font-family: "DM Sans", "Arial", sans-serif;
  font-size: 40px;
  line-height: 46px;
  font-weight: 700;
  text-align: center;

  @media (min-width: 1920px) {
    font-size: 42px;
    line-height: 49px;
  }
}

.nature__text {
  margin-bottom: 43px;
  color: #6f7787;
  font-family: "DM Sans", "Arial", sans-serif;
  font-size: 17px;
  line-height: 24px;
  text-align: center;

  @media (min-width: 1920px) {
    width: 470px;
    margin: 0 auto;
    margin-bottom: 35px;
    font-size: 18px;
    line-height: 28px;
  }
}

.nature__button {
  width: 314px;
  height: 73px;
  padding: 22px 44px;
  border-radius: 45px;

  @media (min-width: 1920px) {
    width: 210;
    height: 64px;
    padding: 20px 44px;
  }
}

.br-desktop {
  display: none;

  @media (min-width: 1920px) {
    display: block;
  }
}
</style>
