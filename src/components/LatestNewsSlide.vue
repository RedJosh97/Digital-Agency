<template>
  <div class="card-template">
    <div class="news-picture">
      <img :src="image" />
    </div>
    <p>{{ title }}</p>
    <p>{{ content }}</p>
  </div>
</template>

<script>
export default {
  name: 'LatestNewsSlide',
  props: {
    image: {
      type: String,
      default: ''
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
.card-template img {
  object-fit: cover;
  width: 80%;
  height: 280px;
  border-radius: 5px;
  padding: 0 1em;
}

.news-picture {
  text-align: center;
}

.card-template p {
  text-align: center;
  color: #515151;
  font-size: 14px;
}
</style>
