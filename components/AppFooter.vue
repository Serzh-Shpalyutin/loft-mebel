<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__top">
        <div class="footer__top-lside">
          <h4 class="footer__top-title">НАВИГАЦИЯ</h4>

          <nav class="footer-top-nav">
            <ul class="footer-top-nav__list list-reset">
              <li class="footer-top-nav__item">
                <nuxt-link class="footer-top-nav__link" to="">Кухни</nuxt-link>
              </li>

              <li class="footer-top-nav__item">
                <nuxt-link class="footer-top-nav__link" to="">Спальни</nuxt-link>
              </li>

              <li class="footer-top-nav__item">
                <nuxt-link class="footer-top-nav__link" to="">Гостинные</nuxt-link>
              </li>

              <li class="footer-top-nav__item">
                <nuxt-link class="footer-top-nav__link" to="">Прихожие</nuxt-link>
              </li>

              <li class="footer-top-nav__item">
                <nuxt-link class="footer-top-nav__link" to="">Офисная мебель</nuxt-link>
              </li>

              <li class="footer-top-nav__item">
                <nuxt-link class="footer-top-nav__link" to="">Детская</nuxt-link>
              </li>

              <li class="footer-top-nav__item">
                <nuxt-link class="footer-top-nav__link" to="">Шкафы</nuxt-link>
              </li>

              <li class="footer-top-nav__item">
                <nuxt-link class="footer-top-nav__link" to="">Матрасы</nuxt-link>
              </li>

              <li class="footer-top-nav__item">
                <nuxt-link class="footer-top-nav__link" to="">Мягкая мебель</nuxt-link>
              </li>
            </ul>
          </nav>
        </div>

        <div class="footer__top-rside">
          <nuxt-link class="footer__top-logo" to="">LM</nuxt-link>

          <address class="footer__top-address">
            г. Анапа, Анапское шоссе, <br>
            30 Ж/К Черное море
          </address>
        </div>
      </div>

      <div class="footer__bottom">
        <div class="footer__bottom-lside">
          <nav class="footer-bottom-nav">
            <ul class="footer-bottom-nav__list list-reset">
              <li class="footer-bottom-nav__item">
                <nuxt-link class="footer-bottom-nav__link" to="">Акция</nuxt-link>
              </li>

              <li class="footer-bottom-nav__item">
                <nuxt-link class="footer-bottom-nav__link" to="">Новинки</nuxt-link>
              </li>
            </ul>
          </nav>
        </div>

        <div class="footer__bottom-rside">
          <ul class="footer-contacts-list list-reset">
            <li class="footer-contacts-list__item">
              <a class="footer-contacts-list__link" href="tel:89648999119">8 (964) 89 99 119</a>
            </li>

            <li class="footer-contacts-list__item">
              <a class="footer-contacts-list__link" href="" target="_blank">INSTAGRAM</a>
            </li>

            <li class="footer-contacts-list__item">
              <a class="footer-contacts-list__link" href="mailto:mebel_loft_anapa@mail.ru">mebel_loft_anapa@mail.ru</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.footer {
  box-shadow: 0 -4px 10px 0 rgba(0, 0, 0, 0.03);
  padding: 55px 0 32px;

  &__top {
    display: flex;
    justify-content: space-between;
    margin-bottom: 35px;
  }

  &__top-lside {
    width: 100%;
  }

  &__top-title {
    font-weight: 500;
    font-size: 14px;
    line-height: 127%;
    color: #000;
    margin-bottom: 10px;
  }

  &__top-logo {
    display: block;
    font-weight: 900;
    font-size: 42px;
    color: #000;
    margin-bottom: 20px;
  }

  &__top-address {
    font-weight: 400;
    font-size: 14px;
    line-height: 127%;
    font-style: normal;
  }

  &__bottom {
    display: flex;
    justify-content: space-between;
  }
}

.footer-top-nav {
  &__list {
    max-width: 400px;
    width: 100%;
    display: grid;
    grid-template-columns: 25% 35% 30%;
    gap: 10px;
  }

  &__item {
    font-weight: 400;
    font-size: 14px;
    line-height: 127%;
  }
}

.footer-bottom-nav {
  &__list {
    display: flex;
  }

  &__item {
    font-weight: 400;
    font-size: 14px;
    line-height: 127%;

    &:first-child {
      color: #d74444;
    }

    &:not(:last-child) {
      margin-right: 30px;
    }
  }
}

.footer-contacts-list {
  display: flex;

  &__item {
    font-weight: 400;
    font-size: 14px;
    line-height: 127%;
    text-align: right;

    &:not(:last-child) {
      margin-right: 30px;
    }
  }
}
</style>