<template>
	<div class="single-container flex-ct-x" data-title="使用clip-path排版蜂窝布局">
		<input id="a" type="checkbox" hidden>
		<input id="b" type="checkbox" hidden>
		<input id="c" type="checkbox" hidden>
		<input id="d" type="checkbox" hidden>
		<div class="cellular-layout" style="--count: 20">
			<label for="a" style="--index: 0">床</label>
			<label class="a" style="--index: 1">前</label>
			<label class="a" style="--index: 2">明</label>
			<label class="a" style="--index: 3">月</label>
			<label class="a" style="--index: 4">光</label>
			<label for="b" style="--index: 5">疑</label>
			<label class="b" style="--index: 6">是</label>
			<label class="b" style="--index: 7">地</label>
			<label class="b" style="--index: 8">上</label>
			<label class="b" style="--index: 9">霜</label>
			<label for="c" style="--index: 10">举</label>
			<label class="c" style="--index: 11">头</label>
			<label class="c" style="--index: 12">望</label>
			<label class="c" style="--index: 13">明</label>
			<label class="c" style="--index: 14">月</label>
			<label for="d" style="--index: 15">地</label>
			<label class="d" style="--index: 16">头</label>
			<label class="d" style="--index: 17">思</label>
			<label class="d" style="--index: 18">故</label>
			<label class="d" style="--index: 119">乡</label>
		</div>
	</div>
</template>

<style lang="scss" scoped>
.single-container {
  padding: 100px 0;
}
.cellular-layout {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin-top: -50px;
  width: 500px;
  text-align: center;
  label {
    --Θ: calc(var(--index) / var(--count) * 1turn);
    margin-left: -15px;
    width: 100px;
    height: 100px;
    background-color: #3c9;
    filter: hue-rotate(var(--Θ));
    clip-path: polygon(25% 5%, 75% 5%, 100% 50%, 75% 95%, 25% 95%, 0 50%);
    cursor: pointer;
    line-height: 100px;
    font-size: 20px;
    color: #fff;
    transition: all 300ms;
    &:nth-child(5n + 2),
    &:nth-child(5n + 4) {
      transform: translateY(50px);
    }
    &:nth-child(4n-3) {
      margin-left: 0;
    }
  }
}
#a:checked ~ .cellular-layout .a {
  opacity: 0;
}
#b:checked ~ .cellular-layout .b {
  opacity: 0;
}
#c:checked ~ .cellular-layout .c {
  opacity: 0;
}
#d:checked ~ .cellular-layout .d {
  opacity: 0;
}
</style>