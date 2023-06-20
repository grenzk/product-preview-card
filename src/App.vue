<template>
  <main>
    <div class="card">
      <picture class="product-img">
        <source srcset="@/assets/img/image-product-desktop.jpg" media="(min-width: 600px)" />
        <img src="@/assets/img/image-product-mobile.jpg" alt="Chanel Perfume" />
      </picture>

      <div class="product-info l-flex">
        <p class="category">Perfume</p>

        <h1 class="title">Gabrielle Essence Eau De Parfum</h1>
        <p class="description">
          A floral, solar and voluptuous interpretation composed by Olivier Polge, Perfumer-Creator
          for the House of CHANEL.
        </p>

        <div class="price l-inline">
          <p class="discount">$149.99</p>
          <p class="original">$169.99</p>
        </div>

        <button class="button">
          <img src="./assets/img/icon-cart.svg" alt="Cart Icon"/>
          <small>Add to Cart</small>
        </button>
      </div>
    </div>
  </main>
</template>

<style lang="scss">
.card {
  display: flex;
  flex-direction: column;
  max-width: 44rem;
  margin: 2rem 1rem;
}

.product-img {
  overflow: hidden;
  border-radius: 0.7rem 0.7rem 0 0;
}

.product-info {
  background-color: hsl(var(--neutral-white));
  border-radius: 0 0 0.7rem 0.7rem;

  .category {
    text-transform: uppercase;
    letter-spacing: 0.4rem;
  }

  .title {
    font-family: var(--heading-font);
    font-size: var(--biggest-font-size);
    color: hsl(var(--neutral-dark-blue));
    line-height: 1;
  }

  .description {
    font-size: var(--h3-font-size);
    line-height: 1.6;
  }

  .price {
    .discount {
      font-family: var(--heading-font);
      font-size: var(--biggest-font-size);
      color: hsl(var(--primary-dark-cyan));
    }

    .original {
      font-size: var(--h3-font-size);
      text-decoration: line-through;
    }
  }

  .button {
    display: flex;
    justify-content: center;
    align-items: center;
    column-gap: 0.9rem;
    padding: 1.1rem;
    color: hsl(var(--neutral-white));
    font-size: var(--h3-font-size);
    background-color: hsl(var(--primary-dark-cyan));
    border: none;
    border-radius: 0.6rem;

    img {
      width: 17px;
    }

    &:hover,
    &:focus {
      background-color: hsl(var(--primary-very-dark-cyan));
    }
  }
}
</style>
