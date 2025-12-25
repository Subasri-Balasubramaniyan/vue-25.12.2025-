<script setup>
import { ref } from 'vue'

const name = ref('')
</script>

<template>
  <div class="user-card">
    <h2>User Profile</h2>

    <input
      v-model="name"
      type="text"
      placeholder="Enter your name"
      class="input"
    />

    <p v-if="name" class="greeting">
      Hello, <span>{{ name }}</span> 👋
    </p>
  </div>
</template>

<style scoped>
.user-card {
  width: 300px;
  padding: 20px;
  border-radius: 12px;
  background: #ffffff;
  box-shadow: 0 6px 14px rgba(0, 0, 0, 0.1);
  margin: 20px auto;
  text-align: center;
}

.input {
  width: 100%;
  padding: 10px 12px;
  font-size: 1rem;
  border: 2px solid #e5e7eb;
  border-radius: 8px;
  outline: none;
  transition: border 0.2s;
}

.input:focus {
  border-color: #4f46e5;
}

.greeting {
  margin-top: 15px;
  font-size: 1.1rem;
  color: #374151;
}

.greeting span {
  font-weight: bold;
  color: #4f46e5;
}
</style>
