<template>
  <div class="content">
    <Header />
    <p class="text-center">Your cart is currently empty.</p>
    <Footer />
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'

export default {
  layout: 'CenteredLayout', 
  components: {
    Header,
    Footer,
  }
}
</script>