<template>
  <div class="container">
    <h1>{{ message }}</h1>
    <p>这是一个简单的 Vue3 项目</p>
    <button @click="count++">点击次数: {{ count }}</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const message = ref('欢迎使用 Vue3!')
const count = ref(0)
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  font-family: Arial, sans-serif;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

h1 {
  color: white;
  font-size: 3em;
  margin: 0;
}

p {
  color: rgba(255, 255, 255, 0.9);
  font-size: 1.2em;
  margin: 10px 0;
}

button {
  margin-top: 20px;
  padding: 12px 24px;
  font-size: 1em;
  background-color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: all 0.3s ease;
}

button:hover {
  transform: scale(1.05);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
}
</style>
