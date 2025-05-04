<template>
    <div class="modal">
      <div class="modal-content">
        <span @click="$emit('close')" class="close-btn">&times;</span>
        <h2>Your Modal</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Exercitationem magni perspiciatis praesentium accusantium inventore voluptas! Similique porro quibusdam, magnam eius voluptatem odio. Voluptates tempore distinctio eveniet suscipit repellendus, fuga obcaecati!</p>
      </div>
    </div>
  </template>
  
  <script lang="ts" setup>
  // Можна додати логіку для модалки, якщо потрібно
  </script>
  
  <style scoped>
  .modal {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .modal-content {
    background: #fff;
    padding: 20px;
    border-radius: 10px;
    width: 300px;
    position: relative;
  }
  
  .close-btn {
    position: absolute;
    top: 10px;
    right: 10px;
    font-size: 24px;
    cursor: pointer;
  }
  </style>
  