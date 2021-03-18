<template>
	<div class="single-container flex-ct-x" data-title="使用repeatig-conic-gradient()描绘墙纸">
    <div class="basis"></div>
	</div>
</template>

<style lang="scss" scoped>
.basis {
  width: 200px;
  height: 200px;
  margin: 50px auto;
  background: repeating-conic-gradient(deeppink 0 15deg, yellowgreen 0 30deg);
  border: 1px solid #000;
}
</style>