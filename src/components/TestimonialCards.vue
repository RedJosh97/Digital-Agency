<template>
  <div class="card">
    <div class="quotation">
      <img src="/image/quotation.png" />
    </div>
    <p>{{ content }}</p>

    <div class="profile-attribute">
      <div class="profile-cover">
        <img class="profile-cover-img" :src="profileImage" />
        <div>
          <p>{{ name }}</p>
          <small>{{ description }}</small>
        </div>
      </div>
      <div class="star-rating">
        <i class="las la-star"></i>
        <i class="las la-star"></i>
        <i class="las la-star"></i>
        <i class="las la-star"></i>
        <i class="las la-star"></i>
        <p>5.0</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TestimonialCards',
  props: {
    bracket: {
      type: String,
      default: ''
    },
    content: {
      type: String,
      default: 'content'
    },
    profileImage: {
      type: String,
      default: ''
    },
    name: {
      type: String,
      default: 'name'
    },
    description: {
      type: String,
      default: 'description'
    }
  }
}
</script>

<style scoped>
.card {
  background: #fff;
  width: 496px;
  min-width: 280px;
  border-radius: 10px;
  padding: 0.4em 1em;
  gap: 26px;
}
.quotation {
  text-align: center;
  margin: 0 auto;
}
.quotation img {
  width: 16px;
}

.card p {
  color: #5f5f5f;
  font-size: 13px;
}
.profile-cover {
  margin-top: 12px;
}

.profile-cover-img {
  margin-right: 17px;
}
.profile-attribute {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
small {
  font-size: 12px;
  color: #5f5f5f;
}
.profile-cover img {
  width: 35px;
}
.star-rating {
  display: flex;
}
.star-rating i {
  color: rgb(249, 249, 3);
  filter: drop-shadow(0px 4px 14px rgba(49, 177, 20, 0.15));
}
.profile-cover {
  display: flex;
  align-items: center;
}

@media (max-width: 800px) {
  .card {
    width: 80%;
  }
}
@media (max-width: 800px) {
  .profile-attribute {
    flex-direction: column;
  }
}
@media (max-width: 700px) {
  .card {
    padding: 1.7em;
  }
}
</style>
