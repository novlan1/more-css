<template>
  <div class="single-container flex-ct-x" data-title="使用mask制作转场动画">
    <div class="img1"></div>
    <div class="img2"></div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style lang='scss' scoped>
.img1 {
  background: url(https://s.newtalk.tw/album/news/111/5a558de0a141b.jpg)
    no-repeat left top;
  background-size: cover;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
}

.img2 {
  position: absolute;
  height: 100%;
  width: 100%;
  left: 0;
  top: 0;
  mask: url(https://i.imgur.com/AYJuRke.png);
  mask-size: 3000% 100%;
  animation: maskMove 2s steps(29) infinite;
}

.img2::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  background: url(https://estnn.com/wp-content/uploads/2020/07/yone-splash-800x450.jpg)
    no-repeat left top;
  background-size: cover;
}

@keyframes maskMove {
  from {
    mask-position: 0 0;
  }
  to {
    mask-position: 100% 0;
  }
}
</style>