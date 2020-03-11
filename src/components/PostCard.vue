<template>
  <div class="card mb-4 shadow-sm">
    <img
      className="bd-placeholder-img card-img-top"
      width="100%"
      height="auto"
      :src="image"
      alt="post background"
    >
    <div class="card-body">
      <h1 class="card-title">
        {{ title }}
      </h1>
      <p class="card-text">
        {{ description }}
      </p>
      <div class="d-flex justify-content-between align-items-center">
        <small class="text-muted">{{ readTime }} mins</small>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: '',
  props: {
    image: {
      type: String,
      default: ''
    },
    title: {
      type: String,
      default: ''
    },
    description: {
      type: String,
      default: ''
    },
    readTime: {
      type: Number,
      default: 0
    }
  }
}
</script>

<style scoped>

</style>
