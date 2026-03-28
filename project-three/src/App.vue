<script setup>
import a from "@/assets/images/a.png";
import src from "@/assets/images/b.avif";
</script>

<template>
  <section>
    <!-- Absolute path to /public folder -->
    <img src="/images/75552.avif" alt="" />
    <img src="/images/premium_photo-1667030474693-6d0632f97029.avif" alt="" />
  </section>

  <section>
    <!-- Relative path to /assets folder -->
    <img src="@/assets/images/75552.avif" alt="" />
    <img
      src="@/assets/images/premium_photo-1667030474693-6d0632f97029.avif"
      alt=""
    />
  </section>

  <section>
    <!-- Import asset into component -->
    <img v-bind:src="a" alt="" />

    <img :src alt="" />
  </section>
</template>

<style scoped>
section {
  display: grid;
  grid-template-columns: 1fr 1fr;
  padding: 10px;
  background: white;
  border-radius: 10px;
}
img {
  width: 100%;
}
</style>
