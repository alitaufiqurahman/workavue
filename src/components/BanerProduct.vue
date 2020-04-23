<template>
  <!-- Women Banner Section Begin -->
  <section class="women-banner spad">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-12 mt-5">
          <carousel
            class="product-slider"
            :items="3"
            :autoplay="true"
            :nav="false"
            :dots="false"
            :autoplaySpeed="2000"
            :autoplayTimeout="5000"
            :loop="true"
          >
            <div class="product-item">
              <div class="pi-pic">
                <img src="img/1.JPG" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="product.html">+ Lihat</a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Bag</div>
                <a href="#">
                  <h5>Name Brand</h5>
                </a>
                <div class="product-price">
                  IDR 480.000
                  <span>IDR 750.000</span>
                </div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="img/2.JPG" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="#">+ Lihat</a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Bag</div>
                <a href="#">
                  <h5>Name Brand</h5>
                </a>
                <div class="product-price">
                  IDR 650.000
                  <span>IDR 550.000</span>
                </div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="img/2@2x.png" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <a href="#">+ Lihat</a>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Bag</div>
                <a href="#">
                  <h5>Name Brand</h5>
                </a>
                <div class="product-price">IDR 750.000</div>
              </div>
            </div>
            <div class="product-item">
              <div class="pi-pic">
                <img src="img/3@2x.png" alt />
                <ul>
                  <li class="w-icon active">
                    <a href="#">
                      <i class="icon_bag_alt"></i>
                    </a>
                  </li>
                  <li class="quick-view">
                    <router-link to="/product">+ Lihat</router-link>
                  </li>
                  <li class="w-icon">
                    <router-link to="/product">
                      <i class="fa fa-random"></i>
                    </router-link>
                  </li>
                </ul>
              </div>
              <div class="pi-text">
                <div class="catagory-name">Bag</div>
                <h5>Name Brand</h5>
                <div class="product-price">IDR 850.000</div>
              </div>
            </div>
          </carousel>
        </div>
      </div>
    </div>
  </section>
  <!-- Women Banner Section End -->
</template>

<script>
import carousel from "vue-owl-carousel";

export default {
  name: "BanerProduct",
  components: {
    carousel
  }
};
</script>

<style scoped>
.product-item {
  margin-right: 25px;
}
</style>