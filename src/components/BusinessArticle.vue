<template>
  <div class="businessContainer">
    <ProductInfo
      title="What we do"
      subTitle="Perfect Solution for Your Business"
      src="/public/image/discount.png"
      description="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever"
    />
    <div class="businessBox">
      <BusinessProps
        :image="'/image/rating 1.svg'"
        title="Grow your business"
        content="we always to help your company to grow with us."
        detailsDefault="Learn More"
        bgColor="#FFE9D6"
      />
      <BusinessProps
        :image="'/image/stats (1) 1.svg'"
        title="Drive more sales"
        content="Every company that we handle we always drive more sales.."
        detailsGreen="Learn More"
        bgColor="#EAFFE7"
      />
      <BusinessProps
        :image="'/image/discount (2) 1.svg'"
        title="Handle by experts"
        content="You don’t need to worry, We are experts.."
        detailsDefault="Learn More"
        bgColor="#FFFCE0"
      />
    </div>
  </div>
</template>

<script>
import ProductInfo from './ProductInfo.vue'
import BusinessProps from './BusinessProps.vue'
export default {
  name: 'BusinessArticle',
  data() {},
  components: {
    BusinessProps,
    ProductInfo
  }
}
</script>

<style scoped>
.businessContainer {
  padding: 2em 6em 2em;
}
.businessBox {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 30px;
  margin-top: 3em;
}

@media (max-width: 800px) {
  .businessBox {
    flex-direction: column;
  }
}
@media (max-width: 700px) {
  .businessContainer {
    padding: 1.7em;
    text-align: center;
  }
}
</style>
