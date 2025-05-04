<script lang="ts" setup>
const emit = defineEmits(['openModal'])

function handleClick (){
emit('openModal')
};
</script>


<template>
    <footer>
      <div class="container">
        <nav class="footer_nav">
          <a class="footer__link" to="/about">Chi siamo</a>
          <a class="footer__link" to="/contact">Contatti</a>
          <a class="footer__link" to="/privacy">Privacy</a>
        </nav>
        <div class="footer__actions">
          <button @click="handleClick" >Contattaci</button>
        </div>
      </div>
    </footer>
  </template>

  <style scoped>
  footer {
    background-color: rgb(92, 107, 122);
    color: #fff;
    padding: 20px;
    text-align: center;
  }
  
  .footer_nav {
    margin-bottom: 10px;
  }
  
  .footer__link {
    color: #fff;
    margin: 0 10px;
    display: flex;
    text-decoration: none;
  }
  
  .footer__link:hover {
    text-decoration: underline;
  }
  
  .footer__actions {
    margin-top: 20px;
  }
  
  
  
  .footer__button:hover {
    background-color: #0056b3;
  }
</style>