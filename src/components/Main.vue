<template>
  <main>
    <section class="jumbotron">
      <div class="container">
        <a href="#">CURRENT SERIES</a>
      </div>
    </section>

    <section class="container">
      <div class="product-card-container">
        <ProductCard/>
        SPAZIO CARD
      </div>

      <a href="#">LOAD MORE</a>
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