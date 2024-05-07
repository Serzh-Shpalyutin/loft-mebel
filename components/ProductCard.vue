<script setup>

</script>

<template>
  <article to="/" class="products-catalog__item product-card">
    <button class="product-card__favs">
      <svg width="19" height="17" viewBox="0 0 19 17" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path
          d="M2.29442 8.54442L9.75 16L17.2056 8.54442C18.0344 7.71562 18.5 6.59152 18.5 5.41942C18.5 2.97864 16.5214 1 14.0806 1C12.9085 1 11.7844 1.46562 10.9556 2.29442L9.75 3.5L8.54442 2.29442C7.71562 1.46562 6.59152 1 5.41942 1C2.97864 1 1 2.97864 1 5.41942C1 6.59152 1.46561 7.71561 2.29442 8.54442Z"
          stroke="black" stroke-linejoin="round" />
      </svg>
    </button>

    <NuxtLink to="/" class="product-card__img">
      <NuxtImg src="img/content/products/product1.png" />
    </NuxtLink>

    <div class="product-card__content">
      <h3 class="product-card__title">Толикс-2 White Gloss</h3>
      <span class="product-card__category">Барные стулья</span>
      <span class="product-card__price">4 690₽</span>
      <button class="product-card__btn">Добавить в корзину</button>
    </div>
  </article>
</template>

<style lang="scss" scoped>
.product-card {
  position: relative;
  padding: 40px 20px 20px 20px;

  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 50px;
  transition: box-shadow .2s ease-in-out;

  &:hover {
    box-shadow: 0 1px 9px 0 rgba(0, 0, 0, 0.11);

    .product-card__btn {
      opacity: 1;
      visibility: visible;
    }
  }

  &__favs {
    position: absolute;
    top: 10px;
    right: 10px;
    background: transparent;
    border: none;
    cursor: pointer;
  }

  &__img {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  &__title {
    font-weight: 500;
    font-size: 16px;
    margin-bottom: 10px;
  }

  span {
    display: block;
  }

  &__category {
    font-weight: 400;
    font-size: 11px;
    margin-bottom: 10px;
  }

  &__price {
    font-weight: 500;
    font-size: 16px;
    margin-bottom: 15px;
  }

  &__btn {
    max-width: 223px;
    width: 100%;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    border: none;
    font-weight: 400;
    font-size: 13px;
    color: #fff;
    background-color: #245462;
    padding: 12px;
    opacity: 0;
    visibility: hidden;
    transition: opacity .2s ease-in-out;
  }
}
</style>