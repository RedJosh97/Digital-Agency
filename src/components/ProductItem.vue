<template>
  <div class="ProductContainer">
    <ProductInfo
      title="About us"
      subTitle="Lorem Ipsum is simply dummy text dummy text"
      buttonLabel="Read More"
    >
      <template #right-section> </template>
    </ProductInfo>

    <div class="framePicture">
      <img src="/image/Rectangle5.png" />
    </div>
    <div class="floatContent">
      <h3>Lorem Ipsum is simply dummy</h3>
      <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
    </div>
  </div>
</template>

<script>
import ProductInfo from './ProductInfo.vue'
export default {
  name: 'ProductItem',
  components: {
    ProductInfo
  }
}
</script>

<style scoped>
.ProductContainer {
  padding: 0 6em;
  background: #fcfcfc;
  position: relative;
}
.framePicture img {
  width: 100%;
  margin-top: 2em;
}
.floatContent {
  border-radius: 7px;
  background: #282c6d;
  width: 22%;
  /* width: 240px; */
  position: absolute;
  bottom: -45px;
  right: 22%;
  padding: 1em 2em;
  color: #e3e3e3;
  font-family: Poppins;
  font-size: 13px;
  line-height: 23px;
}
.floatContent p {
  padding-top: 20px;
}

@media only screen and (max-width: 803px) {
  .floatContent {
    width: 80%;
    position: absolute;
    text-align: center;
    /* margin: 0 auto; */
    display: none;
  }
}

@media (max-width: 700px) {
  .ProductContainer {
    padding: 1.7em;
  }
}
</style>
