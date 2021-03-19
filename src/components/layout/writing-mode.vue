<template>
	<div class="single-container flex-ct-x" data-title="使用writing-mode排版竖向文本">
		<div class="vertical-text">
			<h3>静夜思</h3>
			<p>床前明月光，<br>疑是地上霜。<br>举头望明月，<br>低头思故乡。</p>
		</div>
	</div>
</template>

<style lang="scss" scoped>
.vertical-text {
  writing-mode: vertical-rl;
  h3 {
    padding-left: 20px;
    font-weight: bold;
    font-size: 18px;
    color: #f66;
  }
  p {
    line-height: 30px;
    color: #66f;
  }
}
</style>