<template>
  <div class="businessProps">
    <img :src="image" />
    <h4>{{ title }}</h4>
    <p>{{ content }}</p>
    <button v-if="detailsDefault" class="business-btn">
      {{ detailsDefault }} <i class="las la-arrow-right"></i>
    </button>
    <button v-if="detailsGreen" class="business-green-btn">
      {{ detailsGreen }} <i class="las la-arrow-right"></i>
    </button>
  </div>
</template>

<script>
export default {
  name: 'BusinessProps',
  props: ['title', 'image', 'content', 'detailsDefault', 'detailsGreen']
}
</script>

<style scoped>
.businessProps {
  width: 230px;
  font-family: poppins;
  font-size: 13.7px;
}
.businessProps p {
  margin-top: 1.5em;
  color: #8e8e8e;
}
.business-btn {
  margin-top: 1.5em;
  padding: 7px 13px;
  border: none;
  border-radius: 16px;
  background: #fcfcfc;
  outline: none;
  cursor: pointer;
  margin-left: -12px;
}
.business-green-btn {
  margin-top: 1.5em;
  padding: 7px 13px;
  border: none;
  border-radius: 16px;
  background: green;
  color: #fff;
  outline: none;
  cursor: pointer;
  margin-left: -12px;
}

@media (max-width: 800px) {
  .businessProps {
    width: 100%;
    text-align: center;
  }
}
</style>
