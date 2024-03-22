<script setup>

</script>

<template>
  <nav class="header-middle-nav">
    <ul class="header-middle-nav__list list-reset">
      <li class="header-middle-nav__item">
        <NuxtLink class="header-middle-nav__link" to="/">
          <img src="@/assets/img/svg/wishlist-icon.svg" alt="">
        </NuxtLink>
      </li>

      <li class="header-middle-nav__item">
        <NuxtLink class="header-middle-nav__link" to="/">
          <img src="@/assets/img/svg/bag.svg" alt="">
        </NuxtLink>
      </li>

      <!-- <li class="header-middle-nav__item">
        <NuxtLink class="header-middle-nav__link" to="/">
          <img src="@/assets/img/svg/profile-icon.svg" alt="">
        </NuxtLink>
      </li> -->
    </ul>
  </nav>
</template>

<style lang="scss" scoped>
.header-middle-nav {
  &__list {
    display: flex;
    align-items: center;
    gap: 30px;
  }
}
</style>