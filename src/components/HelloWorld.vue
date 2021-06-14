<template>
  <h1 class="text-yellow-400">{{ msg }}</h1>

  <button
    bg="blue-400 hover:blue-500 dark:blue-500 dark:hover:blue-600"
    text="sm red-400"
    font="mono light"
    p="y-2 x-4"
    border="2 rounded blue-200"
  >
    Button
  </button>

  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank"
      >Vite Documentation</a
    >
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
  </p>

  <button @click="state.count++">count is: {{ state.count }}</button>
  <p>
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<script setup>
import { defineProps, reactive } from "vue";

defineProps({
  msg: String,
});

const state = reactive({ count: 0 });
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
