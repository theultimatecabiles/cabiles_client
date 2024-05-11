<template>
  <div>
    <Header />
    <div class="order-status">
      <div class="order-form">
        <h2 class="heading">Order Status</h2>
        <div class="form-group">
          <label for="orderEmail">Order Email:</label>
          <input type="email" id="orderEmail" v-model="orderEmail" placeholder="Enter your email">
        </div>
        <div class="form-group">
          <label for="orderNumber">Order Number:</label>
          <input type="text" id="orderNumber" v-model="orderNumber" placeholder="Enter your order number">
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
export default {
  data() {
    return {
      orderEmail: '',
      orderNumber: ''
    }
  }
}
</script>

<style scoped>
@import 'assets/css/order-status.css';
</style>