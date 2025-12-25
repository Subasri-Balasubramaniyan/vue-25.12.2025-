<script setup>
import { reactive } from 'vue'

const products = reactive([
  { id: 1, name: 'Laptop', price: 50000 },
  { id: 2, name: 'Phone', price: 20000 },
  { id: 3, name: 'Tablet', price: 15000 },
  { id: 4, name: 'Headphones', price: 3000 }
])
</script>

<template>
  <div class="product-section">
    <h2>Products</h2>

    <div class="product-grid">
      <div
        class="product-card"
        v-for="product in products"
        :key="product.id"
      >
        <h3>{{ product.name }}</h3>
        <p class="price">₹{{ product.price }}</p>
        
      </div>
    </div>
  </div>
</template>

<style scoped>
.product-section {
  max-width: 800px;
  margin: 30px auto;
  padding: 0 15px;
}

.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 20px;
}

.product-card {
  padding: 15px;
  border-radius: 12px;
  background: #ffffff;
  box-shadow: 0 6px 14px rgba(0, 0, 0, 0.1);
  text-align: center;
  transition: transform 0.2s, box-shadow 0.2s;
}

.product-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 18px rgba(0, 0, 0, 0.15);
}

.product-card h3 {
  margin-bottom: 8px;
  color: #111827;
}

.price {
  font-size: 1.1rem;
  font-weight: bold;
  color: #16a34a;
  margin-bottom: 12px;
}

button {
  padding: 8px 14px;
  border: none;
  border-radius: 8px;
  background: #4f46e5;
  color: white;
  cursor: pointer;
  transition: background 0.2s;
}

button:hover {
  background: #4338ca;
}
</style>
