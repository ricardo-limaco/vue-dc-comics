<template>
  <header>
    <div class="container">

      <div class="page-header">
        <a href="#">
          <img src="../assets/dc-logo.png" alt="dc-logo" class="logo">
        </a>
        
        <ul class="navbar">
          <li class="navbar-item" v-for="(item, i) in navbarItems" v-bind:key="i">
            <a href="#">{{ item.title }}</a>
            
          </li>
        </ul>
      </div>

    </div>
  </header>
</template>



<script>
export default {
  name: "Header",
  data() {
    return {
      navbarItems: [
        {title: "Characters"},
        {title: "Comics"},
        {title: "Movie"},
        {title: "Tv"},
        {title: "Games"},
        {title: "Collectibles"},
        {title: "Video"},
        {title: "Fans"},
        {title: "News"},
        {title: "Shop"},
      ]
    }
  }
};
</script>



<style>
</style>