<template>
    <div id="app" class="container">
      <div class="row">
        <div class="col-md-6 mb-3"  v-for="todo in fruitData" :key="todo.id">
          <div class="card" style="width: 100%;"> 
            <div class="card-body" >
              <h5 class="card-title">水果名稱：{{todo.title}}</h5>
              <p class="card-text my-2">價錢：{{todo.price}}</p>
              <p class="card-text mb-3">數量：{{todo.count}}</p>
              <a href="#" class="btn btn-primary">加入購物車</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  <!-- https://codepen.io/su-su-the-sans/pen/NWZpVxN -->
  <!-- 請不要修改下面內容 -->
  <script setup>
    import { ref } from "vue";
  
    const fruitData = ref([
      {id: 1,
        title: 'apple',
        price: 25,
        count: 50,
        imgUrl: 'https://i.imgur.com/w4sYWlS.jpeg'
      },
      {
        id: 2,
        title: 'orange',
        price: 15,
        count: 20,
        imgUrl: 'https://i.imgur.com/PSmzmXi.jpeg'
      },
      {
        id: 3,
        title: 'strawberry',
        price: 45,
        count: 10,
        imgUrl: 'https://i.imgur.com/FIMmh6h.png',
      },
      {
        id: 4,
        title: 'kiwi',
        price: 55,
        count: 20,
        imgUrl: 'https://i.imgur.com/TIA6v4m.jpeg'
      }
    ]);
  </script>