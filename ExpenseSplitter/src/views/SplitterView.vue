<script setup>
import { ref } from 'vue';

const awesome = ref(false);
</script>

<template>
  <main>
    <div id="title">
      <h1>Splitter</h1>
      <button @click="awesome = !awesome">Toggle</button>

      <h3 v-if="awesome">Vue is awesome!</h3>
      <h3 v-else>Oh no 😢</h3>
    </div>
  </main>
</template>

<style scoped>
h1 {
  margin: 0;
  padding: 0;
}
</style>
