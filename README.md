Vue 3 Essentials – Composition API Demo 🚀

This project demonstrates the core concepts of Vue 3 using the Composition API with <script setup>.
It is designed as a learning project to understand the Vue way of thinking.

📌 Concepts Covered

Declarative Rendering ({{ }})

Vue Directives

v-bind (:)

v-on (@)

v-model

v-if, v-show, v-for

Reactivity API

ref() for primitives

reactive() for objects/arrays

Computed Properties

Watchers

Component-based architecture

Scoped component styles

🧩 Features Implemented
🔢 Counter

Increment & decrement buttons

Uses ref() and @click

Styled card UI

👤 User Profile

Username input using v-model

Conditional greeting (v-if)

Styled input field and greeting

🛍️ Product List

Product display using v-for

Uses reactive() array

Responsive grid layout

Styled product cards

📁 Project Structure
vue3-essentials/
│
├── src/
│   ├── components/
│   │   ├── Counter.vue
│   │   ├── UserForm.vue
│   │   └── ProductList.vue
│   │
│   ├── App.vue
│   └── main.js
│
├── index.html
├── package.json
└── README.md

⚙️ Installation & Running the Project
1️⃣ Create the project (Vite)
npm create vite@latest vue3-essentials


Choose:

Framework: Vue

Variant: JavaScript

2️⃣ Install dependencies
cd vue3-essentials
npm install

3️⃣ Run the development server
npm run dev


Open in browser:

http://localhost:5173

📄 Important Files Explained
main.js

Entry point of the application

Mounts App.vue to the DOM

import { createApp } from 'vue'
import App from './App.vue'

createApp(App).mount('#app')

App.vue

Root component

Imports and displays all child components

components/

Each feature is built as a reusable component

Uses <script setup> syntax

Has scoped styles for isolation

🧠 Vue Reactivity Explained
API	Used For
ref()	Numbers, strings, booleans
reactive()	Objects and arrays
computed()	Derived/calculated values
watch()	Side effects (API calls, logs)
🎨 Styling Approach

Pure CSS (no framework)

Scoped styles inside components

Card-based UI

Hover effects and transitions

Responsive layout using CSS Grid

🎯 Learning Outcome

After completing this project, you will understand:

✔ How Vue updates the DOM automatically
✔ How Composition API works
✔ How reactivity is handled internally
✔ How to structure Vue applications
✔ How to build clean, reusable components
