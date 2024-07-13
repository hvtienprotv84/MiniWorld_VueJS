<template>
    <div class="container_news">
    </div>
  </template>
  
  <script>
  export default {
    name: 'MyHeader',
    props: {
      msg: String
    }
  }
  </script>
  
  <style>
  .container_news{
    background-image: url(https://static.miniworldgame.com/nuxts-official-website/public/_nuxt/news-bg.e004853c.png);
    /* background: url() 50%/cover no-repeat; */
background-position: center; /* Vị trí canh giữa */
background-size: 100%; /* Kích thước hình ảnh là 50% của phần tử */
background-repeat: no-repeat; /* Không lặp lại hình ảnh nền */

    /* background-size: 50%; */
    border-bottom-left-radius: .18473rem;
    border-bottom-right-radius: .18473rem;
    height: 100%;
    position: absolute;
    width: 100%;
    margin-top: 1500px;
    left:0;
  }
  </style>
  