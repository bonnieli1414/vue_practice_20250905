<script setup>
import { ref } from "vue";
const text = ref("這是一段文字");
const city = ref("台北市");
const isCheckd = ref(true);
const arrayCheck = ref([]);
const radioValue = ref("男");
</script>

<template>
  <h1>{{ text }}</h1>
  <p>{{ city }}</p>

  <input type="text" v-model="text" />
  <select name="" id="" v-model="city">
    <option value="台北市">台北市</option>
    <option value="台中市">台中市</option>
    <option value="台南市">台南市</option>
  </select>
  <!-- checkbox -->
  <hr />
  {{ isCheckd }}
  <input type="checkbox" name="" id="" v-model="isCheckd" />
  {{ arrayCheck }}
  <input type="checkbox" name="" id="" v-model="arrayCheck" value="大妹" />大妹
  <input type="checkbox" name="" id="" v-model="arrayCheck" value="二妹" />二妹
  <input type="checkbox" name="" id="" v-model="arrayCheck" value="小妹" />小妹
  <!-- radio -->
  {{ radioValue }}
  <input type="radio" name="" id="" v-model="radioValue" value="男" />男
  <input type="radio" name="" id="" v-model="radioValue" value="女" />女
</template>
