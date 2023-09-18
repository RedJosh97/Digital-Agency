<template>
  <div class="testimonial-section">
    <ProductInfo title="Testimonial" subTitle="What customers says about us">
      <template #right-section>
        <div class="select-button">
          <i class="las la-chevron-left left-icon"></i>
          <i class="las la-chevron-right right-icon"></i>
        </div>
      </template>
    </ProductInfo>
    <div class="testimonial-cards">
      <TestimonialCards
        content="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever"
        :profileImage="'/public/image/Ellipse 6-1.png'"
        name="John Peter"
        description="Vue Developer"
      />
      <TestimonialCards
        content="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever"
        :profileImage="'/public/image/Ellipse 6-2.png'"
        name="John Peter"
        description="Ceo, card center"
      />
      <TestimonialCards
        content="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever"
        :profileImage="'/public/image/Ellipse 6-1.png'"
        name="John Peter"
        description="React Developer"
      />
      <TestimonialCards
        content="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever"
        :profileImage="'/public/image/Ellipse 6-1.png'"
        name="John Peter"
        description="React Developer"
      />
    </div>
  </div>
</template>

<script>
import ProductInfo from './ProductInfo.vue'
import TestimonialCards from './TestimonialCards.vue'

export default {
  name: 'TestimonialSetion',
  components: { TestimonialCards, ProductInfo }
}
</script>

<style>
.select-button {
  display: flex;
  gap: 16px;
}

.left-icon,
.right-icon {
  padding: 20px;
  border-radius: 50px;
}

.la-chevron-left {
  color: #04b200;
  background: white;
}
.la-chevron-right {
  color: #fff;
  background: #04b200;
}

.testimonial-cards {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 30px;
  height: auto;
  overflow-x: scroll;
}
.testimonial-cards::-webkit-scrollbar-thumb {
  height: 8px;
  background: #04b200;
  border-radius: 15px;
}

.testimonial-section {
  background: #f1f2fe;
  padding: 3em 6em;
}

@media only screen and (max-width: 850px) {
  .testimonial-cards {
    display: flex;
    flex-direction: column;
  }
}

@media only screen and (max-width: 740px) {
  .cardBox {
    display: flex;
    flex-direction: column;
  }
}
@media (max-width: 700px) {
  .testimonial-section {
    padding: 1.7em;
  }
}
</style>
