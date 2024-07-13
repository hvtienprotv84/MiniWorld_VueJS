<template>
    <div class="container_header">
    <div class="thanh_header">
        <a href="/" class="logo">
            <img src="https://static.miniworldgame.com/nuxts-official-website/public/_nuxt/logo.0edc9054.png" alt="logo">
        </a>
        <ul class="danhmuc">
            <nav>
                <a href="/">
                Trang Chủ
                </a>
            </nav>
            <nav>
                Tin Tức
            </nav>
            <nav>
                Nội Dung Nổi Bật
            </nav>
            <nav>
                WIKI
            </nav>
            <nav>
                MiniStar
            </nav>
            <nav>
                <a href="/" class="language">
            <img src="data:image/png;base64,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" alt="logo">
                </a>
            </nav>
            <nav class="nap">
                <a>Nạp</a>
            </nav>
        </ul>
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
  .container_header{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    
  }
  .thanh_header {
    background-color: #000000b3;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    max-width: 100%;
    height: 85px;
    z-index: 9999;
    display: flex;
    align-items: center;
}
ul{
   color: white;
   display: flex;
   flex-direction: row;
   flex: 1;
   justify-content: space-between;
   max-width: 1000px;
   font-family: cursive;
   font-size: 20px;
}
a{
    text-decoration: none;
    color: white;
}
.logo{
    padding: 50px;    
}
.nap{
    /* background-color: red; */
    background: linear-gradient(90deg, #e1bd38, #fff745);
    width: 205px;
    height: 84px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    right: 0;
    top: 0;
}
.nap a{
    animation: breathe 2s linear infinite;
    color: #262724;
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

.language{
    margin-left: 120px;
}
  </style>
  