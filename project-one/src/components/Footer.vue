<script setup>
import { ref } from "vue";
const year = ref("2026");
const href = ref("https://scrimba.com");
year.value = "2027";
</script>

<template>
  <footer>
    Created by <a v-bind:href="href"><span>Professor Pickle</span></a> &copy;
    {{ year }}
  </footer>
</template>

<style scoped>
footer {
  position: fixed;
  margin: 0 auto;
  bottom: 0;
  text-align: center;
  color: #ccd6d9;
  padding-bottom: 20px;
}

footer span {
  font-family: cursive;
}
a {
  color: white;
}
</style>
