<template>
  <div class="single-container flex-ct-x" data-title="使用mask制作魔幻动画">
    <div class="mask"></div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style lang='scss' scoped>
.single-container {
  width: 100%;
  height: 400px;
  padding: 0;
  filter: contrast(5);
}

.mask {
  position: relative;
  width: 100%;
  height: 100%;
  background: #fff;

  &::before {
    content: "";
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    background: radial-gradient(#000, transparent);
    background-size: 20px 20px;
    mask: repeating-radial-gradient(
      circle at 35% 65%,
      #000,
      rgba(0, 0, 0, 0.5),
      #000 25%
    );
    animation: maskMove 15s infinite linear;
  }
}

@keyframes maskMove {
  @for $i from 0 through 100 {
    #{$i}% {
      mask: repeating-radial-gradient(
        circle at 35% 65%,
        #000,
        rgba(0, 0, 0, 0.5),
        #000 #{$i + 10 + "%"}
      );
    }
  }
}
</style>