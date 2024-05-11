<template>
  <Header />
  <div class="about-us">
    <div class="content">
      <h1 class="title">Online Toy Store</h1>
      <p>We are your one-stop destination for the latest and greatest toys for kids of all ages. From classic favorites to the newest trends, we have something for everyone. Our mission is to provide high-quality toys that inspire creativity, learning, and endless fun.</p>
    </div>
  </div>
  <Footer />
</template>

<script>
import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style scoped>
@import 'assets/css/about-us.css';
</style>