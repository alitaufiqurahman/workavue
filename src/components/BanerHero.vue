<template>
  <!-- Baner Hero Begin -->
  <section class="hero-section">
    <carousel
      class="hero-items"
      :items="1"
      :nav="false"
      :loop="true"
      :autoplay="true"
      :dots="false"
      :autoplaySpeed="5"
    >
      <div class="single-hero-items set-bg" style="background-image: url('/img/3.png')">
        <div class="container">
          <div class="row">
            <div class="col-lg-5 text-white">
              <span>Bag</span>
              <h1 class="text-white">Black Holic</h1>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                do eiusmod tempor incididunt ut labore et dolore
              </p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div>
      </div>
      <div class="single-hero-items set-bg" style="background-image: url('/img/5.jpg')">
        <div class="container">
          <div class="row">
            <div class="col-lg-5 text-white">
              <span>Bag</span>
              <h1 class="text-white">Green Holic</h1>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                do eiusmod tempor incididunt ut labore et dolore
              </p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div>
      </div>
      <div class="single-hero-items set-bg" style="background-image: url('/img/4.jpg')">
        <div class="container">
          <div class="row">
            <div class="col-lg-5 text-white">
              <span>Bag</span>
              <h1 class="text-white">Blue Holic</h1>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                do eiusmod tempor incididunt ut labore et dolore
              </p>
              <a href="#" class="primary-btn">Shop Now</a>
            </div>
          </div>
        </div>
      </div>
    </carousel>
  </section>
  <!-- Baner Hero End -->
</template>

<script>
import carousel from "vue-owl-carousel";

export default {
  name: "BanerHero",
  components: {
    carousel
  }
};
</script>