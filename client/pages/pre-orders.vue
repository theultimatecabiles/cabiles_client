<template>
    <div>
      <Header />
      <div class="container mx-auto px-4 py-8">
        <h1 class="text-4xl font-bold text-gray-800 mb-4">Pre Orders</h1>
        <p class="text-lg text-gray-600 mb-8">This is where you can pre order.</p>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <Pre-orderItem v-for="item in items" :key="item.id" :image="item.image" :title="item.title" :price="item.price" />
        </div>
      </div>
      <Footer />
    </div>
  </template>
  
  <script>
  import Header from '~/components/Header.vue'
  import Footer from '~/components/Footer.vue'

  import android17Image from '~/pictures/dragonball/android17.jpg';
  import krilinImage from '~/pictures/dragonball/krilin.jpg';
  import trunksImage from '~/pictures/dragonball/trunks.jpg';
  
  export default {
    components: {
      Header,
      Footer
    },
    data(){
      return{
        items: [
        { id: 1, image: android17Image, title: 'Dragon Ball GT S.H.Figuarts Super Android 17 Exclusive', price: '₱4500.00' },
        { id: 2, image: krilinImage, title: 'Dragon Ball Z S.H.Figuarts Krillin (Earths Strongest Man)', price: '₱4500.00' },
        { id: 3, image: trunksImage, title: 'Dragon Ball Z S.H.Figuarts Super Saiyan Trunks (Boy from the Future)', price: '₱4500.00' }
        ]
      }
    }
  }
  </script>