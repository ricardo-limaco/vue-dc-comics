<template>
  <div class="product-card">
    <div class="product-card-img">
      <img :src="img" alt="">
    </div>
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