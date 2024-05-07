<script setup>

</script>

<template>
  <section class="products-catalog">
    <div class="container">
      <h2 class="products-catalog__title">Хиты продаж</h2>

      <div class="products-catalog__grid">
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.products-catalog {
  &__title {
    font-weight: 400;
    font-size: 16px;
    color: #343434;
    margin-bottom: 35px;
  }

  &__grid {
    display: grid;
    grid-template-columns: repeat(4, minmax(137px, 263px));
    gap: 50px 30px;
  }
}
</style>