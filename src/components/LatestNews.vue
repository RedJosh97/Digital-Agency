<template>
  <div class="latest-news">
    <ProductInfo title="news" subTitle="Latest news" />

    <div class="cardBox">
      <LatestNewsSlide
        :image="'/image/Rectangle10.png'"
        title="e-commerce"
        content="Lorem Ipsum is simply dummy text of the "
      />
      <LatestNewsSlide
        :image="'/image/Rectangle 18.png'"
        title="e-commerce"
        content="Lorem Ipsum is simply dummy text of the "
      />
      <LatestNewsSlide
        :image="'/image/Rectangle 11.png'"
        title="e-commerce"
        content="Lorem Ipsum is simply dummy text of the "
      />
      <LatestNewsSlide
        :image="'/image/Rectangle 19.png'"
        title="e-commerce"
        content="Lorem Ipsum is simply dummy text of the "
      />
    </div>
  </div>
</template>

<script>
import ProductInfo from './ProductInfo.vue'
import LatestNewsSlide from './LatestNewsSlide.vue'

export default {
  name: 'LatestNews',

  components: { ProductInfo, LatestNewsSlide }
}
</script>

<style scoped>
.latest-news {
  padding: 0 6em 3em;
}
.cardBox {
  display: flex;
  justify-content: space-between;
  gap: 40px;
  margin-bottom: 5em;
}

@media (max-width: 850px) {
  .cardBox {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
}
@media (max-width: 470px) {
  .cardBox {
    grid-template-columns: repeat(1, 1fr);
  }
}
@media (max-width: 700px) {
  .latest-news {
    padding: 1.7em;
  }
}
</style>
