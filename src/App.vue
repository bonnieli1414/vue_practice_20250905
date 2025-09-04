<script setup>
import { ref } from "vue";
const num = ref(2);
function clickMe() {
  num.value++;
}
</script>

<template>
  <h1>練習2025/09/04</h1>
  {{ num }}
  <button type="button" v-on:click="clickMe">點我</button>
</template>
