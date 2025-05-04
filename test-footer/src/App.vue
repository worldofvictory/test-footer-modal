<script setup lang="ts">
import Footer from "./components/Footer.vue";
import Modal from "./components/Modal.vue";
import {ref} from 'vue';

const isShowModal = ref(false)
function showModal(): void {
  isShowModal.value=true
}

</script>

<template>
  <main>
    <h1>Hello</h1>
    <Footer @open-modal="showModal"/>
  <Modal v-if="isShowModal" @close="isShowModal = false" />  
  </main>

</template>

<style scoped>

</style>
