<script setup lang="ts">
import { reactive, ref } from 'vue'

const counter = reactive({
  count: 1
});
const message = ref('hello world!');

counter.count++;



</script>

<template>
  <h2>{{ message }}</h2>
  <h3>当前计算： {{ counter.count }}</h3>
  <button @click="counter.count++">+1</button>
</template>

<style>
</style>
