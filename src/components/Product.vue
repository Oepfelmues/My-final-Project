<script>
import Rating from "./Rating.vue";

export default {
  props: {
    data: Object,
  },
  components: {
    Rating,
  },
};
</script>
<template>
  <div class="card-deck">
  <div class="card">
    <img :src="data.imageUrl" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">{{ data.productName }}</h5>
      <p class="card-text">{{ data.productPrice }}</p>
      <p class="card-text">{{ data.description }}</p>
      <Rating :initalRating="data.rating" />
    </div>
    <div class="card-footer">
      <small class="text-muted">Last updated {{ data.releasedDate }} ago</small>
    </div>
  </div>
  </div>
</template>


