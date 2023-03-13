<template>
  <div class="home">
    <div class="home-text">
      <h1>Welcome to the HiveHouse</h1>

      <p>Discover the best Airbnb stop around. Also know as HouseHive the best Getaway/Over night and simply just a quick Rejuvenate.experience the perfect fusion of Leisure and Pleasure of our Getaways.</p>
      <div class="home-buttons">

        <router-link to="/products" custom v-slot="{ navigate }"><a @click="navigate" role="./ProductView.vue"
            class="btn">Cart</a></router-link>
        <a class="btn">About Us</a>
        <button class="btn" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasBottom"
          aria-controls="offcanvasBottom">Follow Us</button>

        <!--Icons not showing up-->
        <div class="offcanvas offcanvas-bottom" tabindex="-1" id="offcanvasBottom" aria-labelledby="offcanvasBottomLabel">
          <div class="offcanvas-header">
            <h5 class="offcanvas-title mx-auto" id="offcanvasBottomLabel"> Follow us, so that you can stay up to date with the latest Promotions and specials that's available</h5>
            <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
          </div>
          <div class="offcanvas-body large mx-auto">
            <span class="span1"><i class="bi bi-instagram"></i></span>
            <span class="span2"><i class="bi bi-twitter"></i></span>
            <span class="span3"><i class="bi bi-linkedin"></i></span>
          </div>
        </div>

      </div>
    </div>
    <div class="home-img">
      <img src="https://i.postimg.cc/BbRmMbX7/b6ee8c2e0d990997372b3fa12c8d0b24.jpg" class="image1" alt="Landing Image">
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeView from '@/components/HomeView.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>
