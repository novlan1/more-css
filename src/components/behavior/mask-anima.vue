<template>
  <div class="single-container flex-ct-x" data-title="使用mask制作转场动画">
    <div class="mask"></div>
    <div class="mask2"></div>
  </div>
</template>
<style scoped lang='scss'>
.mask,
.mask2 {
  position: relative;
  width: 500px;
  height: 313px;
  &::before {
    position: absolute;
    content: "";
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: url(https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=1877625006,2341162086&fm=26&gp=0.jpg)
      no-repeat;
    background-size: cover;
    z-index: 1;
  }
}

.mask {
  background: url(https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=2128480768,3645204276&fm=26&gp=0.jpg)
    no-repeat;
  background-size: cover;

  &::before {
    animation: maskRotate 4s ease-in-out infinite; // alternate
  }
}
.mask2 {
  margin-left: 40px;
  // background: url(https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=2128480768,3645204276&fm=26&gp=0.jpg) no-repeat;
  // background-size: cover;
  &::before {
    animation: maskRotate2 1.2s linear infinite;
  }
}

@keyframes maskRotate {
  @for $i from 0 through 50 {
    #{$i}% {
      mask: linear-gradient(
        45deg,
        #000 #{$i * 2 + "%"},
        transparent #{$i * 2.5 + "%"},
        transparent #{$i * 2.5 + "%"}
      );
    }
  }
  100% {
    mask: linear-gradient(45deg, #000， #000 100%);
  }
}

@keyframes maskRotate2 {
  @for $i from 0 through 100 {
    #{$i}% {
      mask: conic-gradient(
        #000 #{$i - 8 + "%"},
        transparent #{$i + "%"},
        transparent
      );
    }
  }
}
</style>