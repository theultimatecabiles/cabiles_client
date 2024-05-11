<template>
  <div>
    <Header />
    <div class="container mx-auto px-4 py-8">
      <h1 class="text-4xl font-bold text-gray-800 mb-4">Available Items:</h1>
      <p class="text-lg text-gray-600 mb-8">This is all of the items available.</p>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <ProductItem v-for="item in items" :key="item.id" :image="item.image" :title="item.title" :price="item.price" />
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'
import ProductItem from '~/components/ProductItem.vue';

import wolverineImage from '~/pictures/wolverine.jpg';
import magnetoImage from '~/pictures/magneto.jpg';
import stormImage from '~/pictures/storm.jpg';
import cyclopsImage from '~/pictures/cyclops.jpg';
import jeanImage from '~/pictures/jean.jpg';
import gambitImage from '~/pictures/gambit.jpg';

export default {
  components: {
    Header,
    Footer,
    ProductItem
  },
  data() {
    return {
      items: [
        { id: 1, image: wolverineImage, title: 'Marvel MAFEX No.171 Wolverine (X-Force Ver.)', price: '₱4500.00' },
        { id: 2, image: magnetoImage, title: 'Marvel MAFEX No.179 Magneto (Original Comic Ver.)', price: '₱4500.00' },
        { id: 3, image: stormImage, title: 'Marvel MAFEX No.177 Storm (Comic Ver.)', price: '₱4500.00' },
        { id: 4, image: cyclopsImage, title: 'Marvel MAFEX No.099 Cyclops', price: '₱4500.00' },
        { id: 5, image: jeanImage, title: 'Marvel MAFEX No.160 Jean Grey (Comic Ver.)', price: '₱4500.00' },
        { id: 6, image: gambitImage, title: 'Marvel MAFEX No.131 Gambit (Comic Ver.)', price: '₱4500.00' }
      ]
    }
  }
}
</script>