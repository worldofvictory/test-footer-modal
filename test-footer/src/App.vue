<script setup lang="ts">
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue";
import Modal from "./components/Modal.vue";
import {ref} from 'vue';

const isShowModal = ref(false)
function showModal(): void {
  isShowModal.value=true
}

function seen(){
  const seen="true"
}
function showM(): void {
 seen.value=true
}

</script>

<template>
  <main>
    <Header />
    <p v-if="seen">Ora mi vedi</p>
    <button @click="showM">ok</button>
    <h1>Hello</h1>
    <Footer @open-modal="showModal"/>
  <Modal v-if="isShowModal" @close="isShowModal = false" />  
  </main>

</template>

<style scoped>

</style>
