<script setup>
  defineProps({
    main:{
      type: String,
      default: "this is main content"
    }
  });
</script>

<template>
  <div class="flex justify-center text-center my-5 text-xl">{{main}}</div>
</template>