<script></script>

<template>
  <footer class="footer">
    <a class="footer__arrow" href="#!">
      <span class="visually-hidden">Прокрутить в самое начало.</span>
    </a>
    <a class="footer__logo" href="#!">
      <img src="/images/footer-logo-mobile.svg" width="174" height="66" alt="Наш логотип.">
    </a>
    <ul class="footer__list">
      <li class="footer__item"><a class="footer__link" href="#!">About</a></li>
      <li class="footer__item"><a class="footer__link" href="#!">Pricing</a></li>
      <li class="footer__item"><a class="footer__link" href="#!">Company</a></li>
      <li class="footer__item"><a class="footer__link" href="#!">Blog</a></li>
    </ul>
    <ul class="footer__social-list">
      <li class="footer__social-item">
        <a class="footer__social-link footer__social-link--facebook" href="#!"><span
            class="visually-hidden">Facebook.</span></a>
      </li>
      <li class="footer__social-item">
        <a class="footer__social-link footer__social-link--linkedin" href="#!"><span
            class="visually-hidden">Instagram.</span></a>
      </li>
      <li class="footer__social-item">
        <a class="footer__social-link footer__social-link--google" href="#!"><span
            class="visually-hidden">Google+.</span></a>
      </li>
    </ul>
    <p class="footer__copyright">Copyright © 2019</p>
  </footer>
</template>

<style lang="scss">
.footer {
  padding-top: 148px;
  background-color: #010a20;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;

  @media (min-width: 1440px) {
    flex-direction: row;
    padding: 36px 153px 31px 70px;
  }
}

.footer__arrow {
  position: absolute;
  display: flex;
  top: -41px;
  left: 135px;
  width: 104px;
  height: 104px;
  border-radius: 50%;
  background-color: #dd2242;

  &::before {
    content: "";
    position: absolute;
    display: block;
    width: 38px;
    height: 22px;
    inset: 0;
    margin: auto;
    background-image: url("../images/arrow-up-mobile.svg");
  }

  @media (min-width: 1440px) {
    top: -52px;
    right: 102px;
    display: none;
  }
}

.footer__logo {
  @media (min-width: 1440px) {
    margin-right: 123px;
  }
}

.footer__list {
  margin: 29px 30px 35px;
  display: flex;
  flex-direction: column;
  gap: 36px;
  text-align: center;

  @media (min-width: 1440px) {
    flex-direction: row;
    margin: 0;
    margin-right: auto;
  }
}

.footer__link {
  font-size: 23px;
  line-height: 36px;
  font-weight: 700;
  font-family: "DM Sans", "Arial", sans-serif;
  text-decoration: none;
  color: #ffffff;

  @media (min-width: 1440px) {
    font-size: 18px;
    line-height: 28px;
    letter-spacing: 0.5px;
  }
}

.footer__social-list {
  display: flex;
  gap: 49px;
  margin-bottom: 36px;

  @media (min-width: 1440px) {
    margin-right: 48px;
    margin-bottom: 0;
    gap: 15px;
  }
}

.footer__social-link {
  display: block;
  width: 31px;
  height: 31px;

  &--facebook {
    background-image: url("../images/facebook-mobile.svg");
  }

  &--linkedin {
    background-image: url("../images/linkedin-mobile.svg");
  }

  &--google {
    background-image: url("../images/google-mobile.svg");
  }
}

.footer__copyright {
  margin-bottom: 36px;
  font-family: "DM Sans", "Arial", sans-serif;
  font-size: 24px;
  line-height: 36px;
  font-weight: 700;
  color: #ffffff;
  text-align: center;

  @media (min-width: 1440px) {
    font-size: 18px;
    line-height: 28px;
    margin-bottom: 0;
    margin-right: 10px;
  }
}
</style>
