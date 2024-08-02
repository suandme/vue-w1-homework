<template>
    <div id="app">
      <div class="Q1">
         Ray 身上有 {{RayMoney}} 元，去超商吃午餐花了 {{lunchPrice}} 元，買了一杯飲料花了 {{drinkPrice}} 元
      </div>
  
      <div class="Q2" v-text="rawHTML"></div>
  
      <div class="Q3" v-html="rawHTML"></div>
  
      <div class="Q4" v-once>此欄位為單次綁定 {{ lunchPrice }}</div>
    </div>
  
  </template>
  <!-- https://codepen.io/su-su-the-sans/pen/ExBWJzo -->
  <!-- 請不要修改下面內容 -->
  <script setup>
  import { ref } from "vue";
  
  const RayMoney = ref(1500);
  const lunchPrice = ref(90);
  const drinkPrice = ref(65);
  const rawHTML = ref('<p>姆咪姆咪心動動 (*´∀`)~♥</p>');
  </script>