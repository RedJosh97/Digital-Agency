<template>
  <div class="dialogue-sample">
    <img :src="image" />
    <h4>{{ title }}</h4>
    <p>{{ content }}</p>
  </div>
</template>

<script>
export default {
  name: 'DialogueSample',
  props: {
    image: {
      type: String,
      default: 'image'
    },
    title: {
      type: String,
      default: 'title'
    },
    content: {
      type: String,
      default: 'content'
    }
  }
}
</script>

<style scoped>
.dialogue-sample img {
  width: 100%;
  object-fit: cover;
}
.dialogue-sample h4 {
  color: black;
}
.dialogue-sample {
  color: #5f5f5f;
  font-size: 13px;
  line-height: 25px;
  margin: 0 auto;
  max-width: 500px;
}
</style>
