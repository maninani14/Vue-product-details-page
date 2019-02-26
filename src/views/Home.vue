<template>
  <div class="home mt-5">
    <div class="container-fluid">
      <div class="row justify-content-center">
        <div class="col-md-6">
          <div class="row">
            <div class="col-md-4 col-lg4" v-for="(data,index) in products" :key="index">
              <router-link :to="{ name: 'details', params: { mesaage: products[index] } }">
                <img :src="data.image" class="img-fluid">
                Go to your profile
              </router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return{
      products:[
      {
        productTitle:"Watch- 1",
        image       : require("../assets/products/product-1.png"),
        productId:1
      },
      {
        productTitle:"Watch -2",
        image       : require("../assets/products/product-2.png"),
        productId:2
      }
      ]
    };
  },
  goTodetail() {
    this.$router.go({name: 'details', data: {message: 'Token expired'}});
  }
};
</script>

