<template>
    <div class="container_banner">
        <div class="video">
            <img src="https://static.miniworldgame.com/nuxts-official-website/public/_nuxt/video-btn.f431355c.png"/>
        </div>
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
  .container_banner{
    background-image: url(https://hwimage-cdn.mini1.cn/a/20240524/94906c3d1ae010e9b009686021f76abf.jpg);
    /* background: url() 50%/cover no-repeat; */
    background-position: center; /* Vị trí canh giữa */
    background-size: 100%; /*Kích thước hình ảnh là 50% của phần tử*/
    background-repeat: no-repeat; /* Không lặp lại hình ảnh nền */
    border-bottom-left-radius: 28px;
    border-bottom-right-radius: 28px;
    height: 100%;
    position: absolute;
    width: 100%;
    top: 0;
    left: 0;
  }

  .video{
    display: flex;
    margin: 0 auto;
    margin-top: 370px;
    width: 157px;
    height: 157px;
    animation: breathe 2s linear infinite;

  }
  @keyframes breathe {
  0% {
    transform: scale(1); /* Kích thước ban đầu */
  }
  50% {
    transform: scale(1.1); /* Kích thước lớn lên */
  }
  100% {
    transform: scale(1); /* Trở về kích thước ban đầu */
  }
}  
  </style>
  