<template>
  <div class="product">
    <Header />
    <!-- Breadcrumb Section Begin -->
    <div class="breacrumb-section text-left">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <div class="breadcrumb-text product-more">
              <router-link to="/">
                <i class="fa fa-home"></i> Holic
              </router-link>
              <span>Detail</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Breadcrumb Section Begin -->

    <!-- Product Shop Section Begin -->
    <section class="product-shop spad page-details">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <div class="row">
              <div class="col-lg-6">
                <div class="product-pic-zoom">
                  <img class="product-big-img" :src="gambar_default" alt />
                </div>
                <div class="product-thumbs">
                  <carousel
                    class="product-thumbs-track ps-slider"
                    :items="3"
                    :dots="false"
                    :nav="false"
                    :autoplay="true"
                    :loop="true"
                    :autoplaySpeed="2000"
                  >
                    <div
                      class="pt"
                      @click="changeImage(thumbs[0])"
                      :class="thumbs[0] == gambar_default ? 'active' : '' "
                    >
                      <img src="img/2.JPG" alt />
                    </div>

                    <div
                      class="pt"
                      @click="changeImage(thumbs[1])"
                      :class="thumbs[1] == gambar_default ? 'active' : '' "
                    >
                      <img src="img/3@2x.png" alt />
                    </div>

                    <div
                      class="pt"
                      @click="changeImage(thumbs[2])"
                      :class="thumbs[2] == gambar_default ? 'active' : '' "
                    >
                      <img src="img/2@2x.png" alt />
                    </div>

                    <div
                      class="pt"
                      @click="changeImage(thumbs[3])"
                      :class="thumbs[3] == gambar_default ? 'active' : '' "
                    >
                      <img src="img/1.jpg" alt />
                    </div>
                  </carousel>
                </div>
              </div>
              <div class="col-lg-6">
                <div class="product-details text-left">
                  <div class="pd-title">
                    <span>bag</span>
                    <h3>Name Brand</h3>
                  </div>
                  <div class="pd-desc py-4">
                    <p>
                      Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                      Quam possimus quisquam animi, commodi, nihil voluptate
                      nostrum neque architecto illo officiis doloremque et
                      corrupti cupiditate voluptatibus error illum. Commodi
                      expedita animi nulla aspernatur. Id asperiores blanditiis,
                      omnis repudiandae iste inventore cum, quam sint molestiae
                      accusamus voluptates ex tempora illum sit perspiciatis.
                      Nostrum dolor tenetur amet, illo natus magni veniam quia
                      sit nihil dolores. Commodi ratione distinctio harum
                      voluptatum velit facilis voluptas animi non laudantium, id
                      dolorem atque perferendis enim ducimus? A exercitationem
                      recusandae aliquam quod. Itaque inventore obcaecati, unde
                      quam impedit praesentium veritatis quis beatae ea atque
                      perferendis voluptates velit architecto?
                    </p>
                    <h4>IDR 490.000</h4>
                  </div>
                  <div class="quantity">
                    <router-link to="/cart">
                      <a href="shopping-cart.html" class="primary-btn pd-cart">Add To Cart</a>
                    </router-link>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Product Shop Section End -->

    <RelatedProduct />

    <FooterEnd />
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from "@/components/HelloWorld.vue";
import Header from "@/components/Header.vue";
import FooterEnd from "@/components/FooterEnd.vue";
import RelatedProduct from "@/components/RelatedProduct.vue";

import carousel from "vue-owl-carousel";

export default {
  name: "Product",
  components: {
    Header,
    FooterEnd,
    RelatedProduct,
    carousel
  },
  data() {
    return {
      gambar_default: "img/1.JPG",
      thumbs: ["img/2.JPG", "img/3@2x.png", "img/2@2x.png", "img/1.jpg"]
    };
  },
  methods: {
    changeImage(urlImage) {
      this.gambar_default = urlImage;
    }
  }
};
</script>

<style scoped>
.product-thumbs .pt {
  margin-right: 14px;
}
</style>
