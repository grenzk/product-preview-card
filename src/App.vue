<script setup></script>

<template>
  <main>
    <div class="card">
      <img class="product-img" src="./assets/img/image-product-desktop.jpg" alt="Chanel Perfume" />

      <div class="product-info">
        <p class="category">Perfume</p>

        <h1 class="title">Gabrielle Essence Eau De Parfum</h1>
        <p>
          A floral, solar and voluptuous interpretation composed by Olivier Polge, Perfumer-Creator
          for the House of CHANEL.
        </p>

        <div class="price">
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
  margin: 2rem 1rem;
}

.product-img {
  width: 100%;
  object-fit: cover;
  aspect-ratio: 3 / 2.35;
  border-radius: 1rem 1rem 0 0;
}
</style>
