<template>
	<div class="single-container flex-ct-x" data-title="使用linear-gradient()描绘网格背景">
		<div class="grid-bg"></div>
		<div class="grid-bg-2"></div>
		<div class="grid-bg-3"></div>
	</div>
</template>

<style lang="scss" scoped>
.grid-bg {
  width: 400px;
  height: 400px;
  background-color: #3c9;
  background-image: linear-gradient(0deg, #fff 5%, transparent 5%, transparent),
    linear-gradient(90deg, #fff 5%, transparent 5%, transparent);
  background-position: 0 0, 20px 20px;
  background-size: 20px 20px;
}
.grid-bg-2 {
  background: #58a;
  background-image: linear-gradient(rgba(255, 255, 255, 0.3) 1px, transparent 0),
    linear-gradient(90deg, rgba(255, 255, 255, 0.3) 1px, transparent 0),
    linear-gradient(white 1px, transparent 0),
    linear-gradient(90deg, white 1px, transparent 0);
  background-size: 15px 15px, 15px 15px, 75px 75px, 75px 75px;
  width: 400px;
  height: 400px;
}
.grid-bg-3 {
  background: white;
  background-image: linear-gradient(
      90deg,
      rgba(200, 0, 0, 0.5) 50%,
      transparent 0
    ),
    linear-gradient(rgba(200, 0, 0, 0.5) 50%, transparent 0);
  background-size: 30px 30px;
  width: 400px;
  height: 400px;
}
.grid-bg-2,
.grid-bg-3 {
  margin-left: 40px;
}
</style>