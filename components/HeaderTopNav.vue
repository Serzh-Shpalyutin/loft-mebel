<script setup>

const HeaderTopNav = [
  {
    name: 'Главная',
    link: '/'
  },
  {
    name: 'О нас',
    link: '/about'
  },
  {
    name: 'Контакты',
    link: '/contacts'
  }
];
</script>

<template>
  <nav v-if="HeaderTopNav.length" class="header-top-nav">
    <ul class="header-top-nav__list list-reset">
      <li v-for="item in HeaderTopNav" :key="item.name" class="header-top-nav__item">
        <NuxtLink class="header-top-nav__link" :to="item.link">{{ item.name }}</NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss" scoped>
.header-top-nav {
  &__list {
    display: flex;
    align-items: center;
    gap: 30px;
  }
}
</style>