<template>
    <div id="app">
      <div class="Q1">
        <input type="text" v-model="message" />
      </div>
      <div class="Q2">
        <input type="number" v-model.number="phoneNumber" />
      </div>
    </div>
  </template>
  <!-- https://codepen.io/su-su-the-sans/pen/yLdMWLM -->
  <!-- 請不要修改下面內容 -->
  <script setup>
  import { ref } from "vue";
  
  const message = ref('這是一段話');
  const phoneNumber = ref('0988888888');
  </script>