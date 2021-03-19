<template>
  <div class="single-container flex-ct-x" data-title="使用mask制作多张图片的过渡">
    <div class="mask"></div>
  </div>
</template>
<style scoped lang='scss'>
.mask {
  margin: auto;
  position: relative;
  width: 500px;
  height: 313px;
  background: url(https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=1877625006,2341162086&fm=26&gp=0.jpg)
    no-repeat;
  background-size: cover;

  &::before {
    position: absolute;
    content: "";
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: url(https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=2128480768,3645204276&fm=26&gp=0.jpg)
      no-repeat;
    background-size: cover;
    mask: linear-gradient(45deg, #000 40%, transparent 60%);
    z-index: 1;
  }
}
</style>