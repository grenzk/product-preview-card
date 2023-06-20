<script setup></script>

<template>
  <main>
    <div class="card">
      <img class="product-img" src="./assets/img/image-product-desktop.jpg" alt="Chanel Perfume" />

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
          <img src="./assets/img/icon-cart.svg" />
          <small>Add to Cart</small>
        </button>
      </div>
    </div>
  </main>
</template>

<style lang="scss">
.card {
  border-radius: 1rem;
}

.card {
  display: flex;
  flex-direction: column;
  max-width: 46rem;
  margin: 0 1rem;
}

.product-img {
  width: 100%;
  object-fit: cover;
  aspect-ratio: 3 / 2.35;
  border-radius: 1rem 1rem 0 0;
}

.product-info {
  background-color: hsl(var(--neutral-white));
  border-radius: 0 0 1rem 1rem;

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
    width: 67%;

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
    column-gap: 1rem;
    padding: 1rem;
    color: hsl(var(--neutral-white));
    font-size: var(--h3-font-size);
    background-color: hsl(var(--primary-dark-cyan));
    border: none;
    border-radius: 0.6rem;

    img {
      width: 6%;
    }
  }
}
</style>
