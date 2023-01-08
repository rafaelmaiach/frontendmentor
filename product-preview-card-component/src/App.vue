<template>
  <div class="container">
    <main class="card">
      <picture class="product-picture">
        <source media="(min-width:1440px)" srcset="./assets/image-product-desktop.jpg">
        <img
            class="product-image" src="./assets/image-product-mobile.jpg"
            alt="A Gabrielle Chanel perfume in a square box with yellow liquid inside and some green plants on the edges of the image"
        >
      </picture>
      <div class="content">
        <p class="product-type">perfume</p>
        <h1 class="title fraunces">Gabrielle Essence Eau De Parfum</h1>
        <p class="description">
          A floral, solar and voluptuous interpretation composed by Olivier Polge,
          Perfumer-Creator for the House of CHANEL.
        </p>

        <div class="prices">
          <span class="price-discount fraunces">$149.99</span>
          <del class="price">
            <span class="sr-only">The previous price was</span>
            $169.99
          </del>

        </div>

        <button class="add-cart">
          <img class="add-cart-icon" src="./assets/icon-cart.svg" alt="Cart icon"/>
          <span>Add to Cart</span>
        </button>
      </div>
    </main>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 28px 16px;
}

.card {
  display: flex;
  flex-direction: column;
  border-radius: 10px;
  background-color: var(--pure-white);
  text-align: left;
  max-width: 375px;
}

.content {
  padding: 24px 25px;
}

.product-image {
  width: 100%;
  height: 240px;
  border-top-left-radius: 10px;
  border-top-right-radius: 10px;
}

.product-type {
  font-size: 0.75rem;
  line-height: 15px;
  letter-spacing: 5px;
  margin-bottom: 12px;
  text-transform: uppercase;
}

.title {
  margin-bottom: 16px;
  color: var(--gunmetal);
}

.description {
  font-size: 0.875rem;
  line-height: 23px;
  margin-bottom: 24px;
}

.prices {
  display: flex;
  align-items: center;
  margin-bottom: 24px;
}

.price-discount {
  margin-right: 19px;
  color: var(--deep-aquamarine);
}

.price {
  font-size: 0.8125rem;
  line-height: 23px;
}

.add-cart {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 48px;
  border-radius: 8px;
  padding: 15px 0;
  background-color: var(--deep-aquamarine);
  font-weight: 700;
  font-size: 0.875rem;
  line-height: 17px;
  color: var(--pure-white);
  border: none;
  cursor: pointer;
  transition: background-color 0.2s ease-in-out;
}

.add-cart:hover {
  background-color: var(--deep-aquamarine-dark);
}

.add-cart-icon {
  margin-right: 12px;
  width: 14px;
  height: 16px;
}

@media (min-width: 90em) {
  .container {
    min-height: 100vh;
    justify-content: center;
    padding: 0;
  }

  .content {
    width: 50%;
    padding: 32px;
  }

  .card {
    max-width: 600px;
    height: 450px;
    flex-direction: row;
  }

  .product-picture {
    width: 50%;
  }

  .product-image {
    height: 100%;
    border-top-right-radius: 0;
    border-bottom-left-radius: 10px;
  }

  .product-type {
    margin-bottom: 20px;
  }

  .title {
    margin-bottom: 24px;
  }

  .description {
    margin-bottom: 29px;
  }

  .prices {
    margin-bottom: 30px;
  }
}
</style>
