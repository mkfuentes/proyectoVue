<template>
  <div id="app">
    <Navbar title="Kodium" />
    <section class="container" />
  </div>
</template>

<script>

import Navbar from './components/Navbar'
// import PostCard from './components/PostCard'

export default {
  name: 'Kodium',
  components: {
    Navbar
  },
  data () {
    return {
      posts: []
    }
  },
  async mounted () {
    const response = await fetch('http://localhost:8080/posts')

    const payload = await response.json()

    this.posts = payload.data.posts
  }
}
</script>

<style src="bootstrap/dist/css/bootstrap.min.css">
</style>
