<template>
  <header class="bg-gray-800 py-4">
    <div class="container mx-auto px-4 flex justify-between items-center">
      <h1 class="text-2xl font-semibold text-white">Online Toy Store</h1>
      <nav>
        <ul class="flex space-x-4 justify-center text-white ">
          <li><nuxt-link to="/">Home</nuxt-link></li>
          <li><nuxt-link to="/pre-orders">Pre Orders</nuxt-link></li>
          <li><nuxt-link to="/cart">Cart</nuxt-link></li>
          <li><nuxt-link to="/order-status">Order Status</nuxt-link></li>
          <li><nuxt-link to="/about-us">About Us</nuxt-link></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
}
</script>

<style scoped>
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

nav ul {
  display: flex;
  justify-content: center;
  list-style: none;
  padding: 0;
  margin: 0;
}

nav ul li {
  margin-right: 10px;
}

nav ul li:last-child {
  margin-right: 0;
}
</style>