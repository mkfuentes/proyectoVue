<template>
  <nav class="navbar navbar-light bg-light">
    <span class="navbar-brand mb-0 h1">
      {{ title }}
    </span>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
  props: {
    title: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped>

</style>
