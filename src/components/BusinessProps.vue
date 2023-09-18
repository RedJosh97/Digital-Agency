<template>
  <div class="businessProps">
    <div class="img-wrapper" :style="{ background: `${bgColor}` }">
      <img :src="image" />
    </div>
    <div class="business-props-wrapper">
      <h2>{{ title }}</h2>
      <p>{{ content }}</p>
    </div>
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

  props: {
    title: {
      type: String
    },
    image: {
      type: String
    },
    content: {
      type: String
    },
    detailsDefault: {
      type: String
    },
    detailsGreen: {
      type: String
    },
    bgColor: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped>
.businessProps {
  width: 230px;
  font-family: poppins;
  font-size: 13.7px;
}

.business-props-wrapper {
  margin-top: 2.5em;
  margin-bottom: 2.5em;
}
.business-props-wrapper p {
  margin-top: 2.5em;
  color: #8e8e8e;
}
.img-wrapper {
  border-radius: 10px;
  height: 100px;
  width: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.business-btn {
  padding: 7px 13px;
  border: none;
  border-radius: 16px;
  background: #fcfcfc;
  outline: none;
  cursor: pointer;
  margin-left: -12px;
}
.business-green-btn {
  /* margin-top: 1.5em; */
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
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-align: center;
  }
}
</style>
