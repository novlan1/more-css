

<template>
	<div class="single-container flex-ct-x" data-title="使用conic-gradient()描绘动画">
    <div class="basis"></div>
	</div>
</template>

<style lang="scss" scoped>
@function randomNum($max, $min: 0, $u: 1) {
  @return ($min + random($max)) * $u;
}

@function randomConicGradient() {
  $n: random(30) + 10;
  $list: ();

  @for $i from 0 to $n {
    $list: $list, rgb(randomNum(255), randomNum(255), randomNum(255));
  }

  @return conic-gradient($list, nth($list, 1));
}

.basis {
  position: absolute;
  top: 50%;
  left: 50%;
  margin: -100vmax;
  width: 200vmax;
  height: 200vmax;
  background: randomConicGradient();
  animation: rotate 6s ease-in-out infinite;
}

@keyframes rotate {
  to {
    transform: rotate(1turn);
  }
}
</style>