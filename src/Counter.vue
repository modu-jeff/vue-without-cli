<template>
  <h1 class="count">{{ count }}</h1>
  <button type="button" @click="decrement">-1</button>
  <button type="button" @click="increment">+1</button>
</template>

<script lang="ts" setup>
import { ref } from 'vue';

const count = ref(0);

const increment = (e: Event) => {
  e.preventDefault();
  count.value++;
};
const decrement = (e: Event) => {
  e.preventDefault();
  count.value--;
};
</script>
