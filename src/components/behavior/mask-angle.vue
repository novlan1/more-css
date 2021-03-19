<template>
  <div class="single-container flex-ct-x" data-title="使用mask对图片进行切角">
    <div class="angle"></div>
    <div class="mask"></div>
  </div>
</template>
<style scoped>
.angle {
  width: 200px;
  height: 120px;
  background: linear-gradient(135deg, transparent 15px, deeppink 0) top left,
    linear-gradient(-135deg, transparent 15px, deeppink 0) top right,
    linear-gradient(-45deg, transparent 15px, deeppink 0) bottom right,
    linear-gradient(45deg, transparent 15px, deeppink 0) bottom left;
  background-size: 50% 50%;
  background-repeat: no-repeat;
}
.mask {
  width: 200px;
  height: 120px;
  margin-left: 20px;
  background: url(https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=1877625006,2341162086&fm=26&gp=0.jpg)
    no-repeat;
  background-size: cover;
  mask: linear-gradient(135deg, transparent 15px, #fff 0) top left,
    linear-gradient(-135deg, transparent 15px, #fff 0) top right,
    linear-gradient(-45deg, transparent 15px, #fff 0) bottom right,
    linear-gradient(45deg, transparent 15px, #fff 0) bottom left;
  mask-size: 50% 50%;
  mask-repeat: no-repeat;
}
</style>