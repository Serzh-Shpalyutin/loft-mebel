
import { HeaderCategoriesNav } from '#build/components';
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

    <div class="container header__middle">
      <AppLogo />

      <HeaderSearch />

      <HeaderMiddleNav />
    </div>

    <div class="container header__bottom">
      <HeaderCategoriesNav />
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header {
  color: #fff;

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

    a {
      font-weight: 400;
      font-size: 14px;
    }
  }

  &__middle {
    padding: 20px 15px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 5px;
  }
}
</style>