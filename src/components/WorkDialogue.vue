<template>
  <div class="work-dialogue">
    <ProductInfo title="Our Works" subTitle="Here our few our works" buttonLabel="View More" />

    <div class="dialogue-sample-props">
      <DialogueSample
        :image="'/image/Rectangle 11 (2).png'"
        title="Food Delivery App"
        content="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever"
      />
      <DialogueSample
        :image="'/image/Rectangle 13.png'"
        title="E pay App"
        content="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever"
      />
      <DialogueSample
        :image="'/image/Rectangle 14.png'"
        title="Podcast App"
        content="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever"
      />
      <DialogueSample
        :image="'/image/Rectangle 12.png'"
        title="Service Provider App"
        content="Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever"
      />
    </div>
  </div>
</template>

<script>
import DialogueSample from './DialogueSample.vue'
import ProductInfo from './ProductInfo.vue'
export default {
  name: 'WorkDialogue',
  components: {
    DialogueSample,
    ProductInfo
  }
}
</script>

<style scoped>
.work-dialogue {
  padding: 1.5em 6em;
}

.dialogue-sample-props {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  align-self: self-start;
  align-items: flex-end;
  gap: 40px;
  padding-bottom: 4em;
}

@media (max-width: 1245px) {
  .dialogue-sample-props {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
}
@media (max-width: 530px) {
  .dialogue-sample-props {
    display: block;
  }
}

@media (max-width: 700px) {
  .work-dialogue {
    padding: 0 1rem;
  }
}
</style>
