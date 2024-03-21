<template>
  <header class="header">
    <div class="header__top">
      <div class="container header__top-container">
        <HeaderTopNav />

        <div class="header__top-tel">
          <img src="@/assets/img/svg/phone.svg" alt="">
          <a href="tel:89648999119">8 (964) 89 99 119</a>
        </div>
      </div>
    </div>

    <div class="container header__middle"></div>

    <div class="container header__bottom"></div>
  </header>
</template>

<style lang="scss" scoped>
.header {
  &__top {
    background-color: #313131;
    padding: 11px 0;
  }

  &__top-tel,
  &__top-container {
    display: flex;
    justify-content: space-between;
  }

  &__top-tel {
    img {
      margin-right: 10px;
    }
  }
}
</style>