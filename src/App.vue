<script setup>
import { ref } from "vue";
const name = ref("Agnes");
const emoji = "👌";
</script>

<template>
  <header>
    <span>{{ emoji }}</span>
  </header>
  <main>
    <h1>Hello, {{ name }}!</h1>
    <p>
      I am about to learn
      <a href="https://vuejs.org/" target="_blank">Vue.js</a>!
    </p>
  </main>
  <footer>
    <p>&copy; 2026</p>
  </footer>
</template>

<style scoped>
header span {
  font-size: 3rem;
}
main a {
  color: #428883;
}
footer {
  position: fixed;
  bottom: 0;
  padding-bottom: 20px;
}
</style>
