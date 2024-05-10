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
.order-status {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 70vh;
}

.order-form {
  width: 550px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
  background-color: #fff;
}

.heading {
  font-size: 50px; 
  font-weight: bold; 
  margin-bottom: 20px; 
}

.form-group {
  margin-bottom: 15px;
}

label {
  display: block;
  margin-bottom: 5px;
}
</style>