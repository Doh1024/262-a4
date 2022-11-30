<script setup>
  defineProps({
    pageName: String,
  });
</script>

<template>
  <header class="flex justify-center text-3xl">
    <h1>{{pageName}}</h1>
  </header>
</template>