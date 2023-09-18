<template>
  <div class="top-section-wrapper">
    <div class="title-and-subtitle-wrapper">
      <slot name="left-section">
        <p class="title">{{ title }}</p>
        <h3 class="subtitle">{{ subTitle }}</h3>
      </slot>
    </div>

    <div class="right-section-wrapper">
      <slot name="right-section">
        <p v-if="description" class="description">{{ description }}</p>
        <a class="btn" v-if="buttonLabel">{{ buttonLabel }} <i class="las la-arrow-right"></i> </a>
      </slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProductInfo',
  props: {
    title: {
      type: String,
      default: 'Title'
    },
    subTitle: {
      type: String,
      default: 'subTitle'
    },
    description: {
      type: String
    },
    buttonLabel: {
      type: String,
      default: ''
    }
  }
}
</script>
<style>
.top-section-wrapper {
  padding: 3em 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 40px;
}
.title-and-subtitle-wrapper {
  flex: 1 1 40%;
  display: flex;
  flex-direction: column;
  gap: 20px;
  /* max-width: 476px; */
}

.title {
  color: #ff5325;
}

.subtitle {
  font-size: 30px;
  font-weight: 600;
}

.right-section-wrapper {
  flex: 1 1 60%;
  display: flex;
  justify-content: flex-end;
}
.description {
  max-width: 506px;
}
.btn {
  display: flex;
  padding: 15px 25px;
  background: #e1ffe0;
  color: #04b200;
  border-radius: 6px;
  font-size: 14px;
  align-items: center;
  cursor: pointer;
  /* align-self: flex-end; */
}

@media only screen and (max-width: 850px) {
  .top-section-wrapper {
    display: flex;
    flex-direction: column;
    text-align: center;
  }
}
</style>
