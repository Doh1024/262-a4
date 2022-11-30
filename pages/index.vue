<script setup>
  let products = [
    {
      title: "Jordan 4 Retro A Ma Maniére Violet Ore",
      image:{
        src: "/images/j4.webp",
        alt: "Jordan 4 Retro",
      },
      url: "https://stockx.com/air-jordan-4-retro-a-ma-maniere-violet-ore",
      color: "bg-brown-300"
    },
    {
      title: "Nike Dunk Low Retro White Black Panda (2021)",
      image:{
        src: "/images/panda.png",
        alt: "Nike Dunk Low Retro",
      },
      url: "https://stockx.com/nike-dunk-low-retro-white-black-2021",
      color: "bg-black-200"
    },
    {
      title: "Jordan 1 Retro High Dark Mocha",
      image:{
        src: "/images/j1.webp",
        alt: "Jordan 1 Retro High",
      },
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
        :image="product.image"
        :url="product.url"
        :buttonColor="product.color"
      />
    </div>
  </main>
</template>