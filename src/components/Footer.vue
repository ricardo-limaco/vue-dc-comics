<template>
  <footer>
    <!-- Footer Top -->
    <div class="page-footer-top">
      <div class="container">
        
        <div class="row">

          <div class="col-5-footer" v-for="(item, i) in footerTop" v-bind:key="i">
            <img v-bind:src="item.img" alt="img">
            
            <a href="#"><h3>{{ item.title }}</h3></a>
          </div>
        </div>

      </div>
    </div>


    <!-- Footer Center -->
    <div class="page-footer-center">
      <div class="container">

        <section class="footer-logo">
          <ul class="footer-dc-comics-shop">
            <ul class="footer-dc-comics">
              <li><a href="#"><h4>DC COMICS</h4></a></li>
              <li v-for="(text, i) in footerDcComics" v-bind:key="i">
                <a href="#">{{ text.title }}</a>
              </li>
            </ul>
            
            <ul class="footer-shop">
              <li><a href="#"><h4>SHOP</h4></a></li>
              <li v-for="(text, i) in footerShop" v-bind:key="i">
                <a href="#">{{ text.title }}</a>
              </li>
            </ul>
          </ul>

          <ul class="footer-dc">
            <li><a href="#"><h4>DC</h4></a></li>
            <li v-for="(text, i) in footerDc" v-bind:key="i">
              <a href="#">{{ text.title }}</a>
            </li>
          </ul>

          <ul class="footer-sites">
            <li><a href="#"><h4>SITES</h4></a></li>
            <li v-for="(text, i) in footerSites" v-bind:key="i">
              <a href="#">{{ text.title }}</a>
            </li>
          </ul>

          

        </section>
      </div>
    </div>


    <!-- Footer Bottom -->
    <div class="page-footer-bottom">
      <div class="container">

        <div class="padding">
          <a href="#" class="button">Sign-up now!</a>
          
          <div class="follow">
            <h3>FOLLOW US</h3>
            <ul>
              <li><a href="#"><img src="../assets/footer-facebook.png" alt=""></a></li>
              <li><a href="#"><img src="../assets/footer-twitter.png" alt=""></a></li>
              <li><a href="#"><img src="../assets/footer-youtube.png" alt=""></a></li>
              <li><a href="#"><img src="../assets/footer-pinterest.png" alt=""></a></li>
              <li><a href="#"><img src="../assets/footer-periscope.png" alt=""></a></li>
            </ul>
          </div>

        </div>

      </div>
    </div>

  </footer>
</template>




<script>
export default {
  name: "Footer",
  data() {
    return {
      footerTop: [
        {
          title: "Digital Comics",
          img: require("../assets/buy-comics-digital-comics.png")
        },
        {
          title: "DC Merchandise",
          img: require("../assets/buy-comics-merchandise.png")
        },
        {
          title: "Subscription",
          img: require("../assets/buy-comics-subscriptions.png")
        },
        {
          title: "Comics Shop Locator",
          img: require("../assets/buy-comics-shop-locator.png")
        },
        {
          title: "DC Power Visa",
          img: require("../assets/buy-dc-power-visa.svg")
        },
      ],
      footerDcComics: [
        {title: "Characters"},
        {title: "Comics"},
        {title: "Movies"},
        {title: "TV"},
        {title: "Game"},
        {title: "Video"},
        {title: "News"},
      ],
      footerDc: [
        {title: "Terms OF Use"},
        {title: "Privacy policy (New)"},
        {title: "Ad Choices"},
        {title: "Advertising"},
        {title: "Jobs"},
        {title: "Subscriptions"},
        {title: "Talent Workshops"},
        {title: "CPSC Certificates"},
        {title: "Ratings"},
        {title: "Shop Help"},
        {title: "Contact Us"},
      ],
      footerSites: [
        {title: "DC"},
        {title: "MAD Magazine"},
        {title: "DC Kids"},
        {title: "DC Universe"},
        {title: "DC Power Visa"},
      ],
      footerShop: [
        {title: "SHOP DC"},
        {title: "SHOP DC Collectibles"},
      ]
    }
  }
};
</script>



<style>
</style>