<template>
    <div :id="dynamicId">hello </div>
    <p> ID Corent: {{ dynamicId }}</p>
    <button @click="changeId">Change ID</button>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  // Реактивна змінна
  const dynamicId = ref('initial-id')
  
  const changeId = () => {
  const random = Math.floor(Math.random() * 1000)
  dynamicId.value = random
}
  </script>