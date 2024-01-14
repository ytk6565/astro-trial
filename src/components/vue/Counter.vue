<template>
  <div>
    <h1>Vue Counter: {{ count }}</h1>
    <button @click="increment">Increment</button>
    <button @click="decrement">Decrement</button>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";

const count = ref<number>(0);

const increment = () => {
  count.value++;
};

const decrement = () => {
  count.value--;
};
</script>
