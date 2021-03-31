<template>
	<div class="single-container flex-ct-x" data-title="使用box-shadow描绘单侧投影">
    <div class="wrap">
      <p>所有字体都是条纹字</p>
      <p>利用线性渐变背景实现</p>
      <p>重点在于渐变色白色与透明色的重复渐变</p>
      <p>结合其他CSS属性有很多作用，譬如立体条纹字</p>
    </div>
	</div>
</template>

<style lang="scss" scoped>
.wrap {
  width: 700px;
}
p {
  position: relative;
  text-align: center;
  font-size: 28px;
  line-height: 33px;

  &::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: linear-gradient(
      45deg,
      #fff 0%,
      #fff 25%,
      transparent 25%,
      transparent 50%,
      #fff 50%,
      #fff 75%,
      transparent 75%,
      transparent 100%
    );
    background-size: 6px 6px;
    z-index: 1;
  }
}
</style>