<template>
  <main>
    <section class="jumbotron">
      <div class="container">
        <a href="#" class="btn-large">CURRENT SERIES</a>
      </div>
    </section>

    <section class="container">
      <div class="product-card-container">
        <ProductCard
        v-for="(product, i) in dcList" :key="i" :img="product.thumb" :title="product.series">
        </ProductCard>
        
      </div>

      <div class="btn-small">
        <a href="#">LOAD MORE</a>
      </div>
    </section>
    
  </main>
</template>

<script>
import ProductCard from "./ProductCard.vue";
import jsonData from "../database/dc-comics.json";

export default {
  name: "Main",
  components: {
    ProductCard,
  },
  data() {
    return {
      dcList: jsonData,
    }
  }
};
</script>

<style>

</style>