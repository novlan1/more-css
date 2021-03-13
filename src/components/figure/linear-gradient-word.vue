<template>
	<div class="single-container flex-ct-x" data-title="使用linear-gradient()控制渐变文本">
		<h1 class="gradient-text">SEIZE THE DAY</h1>
	</div>
</template>

<style lang="scss" scoped>
.gradient-text {
  background-image: linear-gradient(90deg, #f66, #f90);
  background-clip: text;
  line-height: 60px;
  font-size: 60px;
  color: transparent;
  animation: hue 5s linear infinite;
}
@keyframes hue {
  from {
    filter: hue-rotate(0);
  }
  to {
    filter: hue-rotate(-1turn);
  }
}
</style>