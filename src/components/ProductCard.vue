<template>
  <div class="product-card">
    <img :src="img" alt="">
    <h4>{{title}}</h4>
  </div>
</template>



<script>
export default {
  name: "ProductCard",
  props: {
    img: String,
    title: String,

  }
};
</script>



<style>
</style>