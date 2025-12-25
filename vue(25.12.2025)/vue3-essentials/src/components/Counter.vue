<script setup>
import { ref } from 'vue'

const count = ref(0)

const increment = () => {
  count.value++
}

const decrement = () => {
  count.value--
}
</script>

<template>
  <div class="counter-card">
    <h2>Counter</h2>

    <p class="count">{{ count }}</p>

    <div class="buttons">
      <button @click="decrement">-</button>
      <button @click="increment">+</button>
    </div>
  </div>
</template>

<style scoped>
.counter-card {
  width: 250px;
  padding: 20px;
  border-radius: 10px;
  background: #f4f6fb;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  text-align: center;
  margin: 20px auto;
}

.count {
  font-size: 2.5rem;
  font-weight: bold;
  margin: 15px 0;
  color: #333;
}

.buttons {
  display: flex;
  justify-content: center;
  gap: 10px;
  padding:10px;
  background-color:white
}

button {
  font-size: 1.5rem;
  border: none;
  border-radius: 50%;
  cursor: pointer;
  background:white;
  color:black;
  transition: transform 0.2s, background 0.2s;
}

button:hover {
  background:white;
  transform: scale(1.1);
}
</style>
