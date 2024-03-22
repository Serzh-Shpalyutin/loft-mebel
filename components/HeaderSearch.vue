<template>
  <div class="header-search">
    <form class="header-search__form">
      <button class="header-search__btn btn-reset">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path
            d="M15 15L11 11M7 13C3.68629 13 1 10.3137 1 7C1 3.68629 3.68629 1 7 1C10.3137 1 13 3.68629 13 7C13 10.3137 10.3137 13 7 13Z"
            stroke="black" />
        </svg>
      </button>

      <label>
        <input class="header-search__input" type="search" placeholder="Поиск">
      </label>
    </form>
  </div>
</template>

<style lang="scss" scoped>
.header-search {
  max-width: 839px;
  width: 100%;

  &__form {
    position: relative;

  }

  &__input {
    padding: 10px 10px 10px 50px;
    width: 100%;
    height: 50px;
    border: 1px solid #E6E6E6;
    border-radius: 0px;
    color: #000;
    font-weight: 400;
    font-size: 14px;

    &::placeholder {
      color: #000;
      font-weight: 400;
      font-size: 14px;
    }
  }

  &__btn {
    position: absolute;
    top: 50%;
    left: 0px;
    transform: translateY(-50%);
    width: 50px;
    height: 50px;
  }
}
</style>