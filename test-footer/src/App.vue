<script setup lang="ts">

</script>

<template>
  <footer>
    <div class="container">
      <nav class="footer_nav">
        <a to="/about">Chi siamo</a>
        <a to="/contact">Contatti</a>
        <a to="/privacy">Privacy</a>
      </nav>
      <div class="footer__actions">
        <button @click="handleClick">Contattaci</button>
      </div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  background-color: lightslategrey;
  color: #fff;
  padding: 20px;
  text-align: center;
}

.footer__nav {
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

.footer_btn {
  background-color: #007bff;
  color: red;
  border: none;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
}

.footer__button:hover {
  background-color: #0056b3;
}
</style>
