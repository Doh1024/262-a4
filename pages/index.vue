<script setup>
  let products = [
    {
      title: "Jordan 4 Retro A Ma Maniére Violet Ore",
      src: "Jordan 4 Retro",
      alt: "https://images.stockx.com/images/Air-Jordan-4-Retro-A-Ma-Maniere-Violet-Ore-Product.jpg?fit=fill&bg=FFFFFF&w=140&h=75&fm=avif&auto=compress&dpr=1&trim=color&updated_at=1668668640&q=80",
      url: "https://stockx.com/air-jordan-4-retro-a-ma-maniere-violet-ore",
      color: "bg-brown-300"
    },
    {
      title: "Nike Dunk Low Retro White Black Panda (2021)",
      src: "Nike Dunk Low Retro",
      alt: "https://images.stockx.com/images/Nike-Dunk-Low-Retro-White-Black-2021-Product.jpg?fit=fill&bg=FFFFFF&w=140&h=75&fm=avif&auto=compress&dpr=1&trim=color&updated_at=1633027409&q=80",
      url: "https://stockx.com/nike-dunk-low-retro-white-black-2021",
      color: "bg-black-200"
    },
    {
      title: "Jordan 1 Retro High Dark Mocha",
      src: "Jordan 1 Retro High",
      alt: "https://images.stockx.com/images/Air-Jordan-1-Retro-High-Dark-Mocha-2-Product.jpg?fit=fill&bg=FFFFFF&w=140&h=75&fm=avif&auto=compress&dpr=1&trim=color&updated_at=1616187367&q=80",
      url: "https://stockx.com/air-jordan-1-retro-high-dark-mocha",
      color: "bg-brown-500"
    }
  ];
</script>

<template>
  <main class="mx-auto">
    <PageHeader pageName="Home page"/>
    <div class="container flex justify-center my-7">
      <AppCard
        v-for="product in products"
        :key="product.id"
        :title="product.title"
        :src="product.src"
        :alt="product.alt"
        :url="product.url"
        :buttonColor="product.color"
      />
    </div>
  </main>
</template>