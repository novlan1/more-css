<template>
	<div class="single-container flex-ct-x" data-title="使用conic-gradient()实现颜色表盘">
    <div class="rainbow"></div>
    <div class="colors"></div>
  </div>
</template>

<style lang="scss" scoped>
$rainbows: (red, orange, yellow, green, teal, blue, purple);
$colors: ();
$totalStops: 20;

// hsl() 被定义为色相-饱和度-明度（Hue-saturation-lightness）
// 色相（H）是色彩的基本属性，就是平常所说的颜色名称，如红色、黄色等。
// 饱和度（S）是指色彩的纯度，越高色彩越纯，低则逐渐变灰，取0-100%的数值。
// 明度（V），亮度（L），取0-100%。

@for $i from 0 through $totalStops {
  $colors: append($colors, hsl($i * (360deg / $totalStops), 100%, 50%), comma);
}

.rainbow {
  width: 200px;
  height: 200px;
  background: conic-gradient($rainbows);
  border-radius: 50%;
}

.colors {
  width: 200px;
  height: 200px;
  background: conic-gradient($colors);
  border-radius: 50%;
}

.rainbow,
.colors {
  margin: 20px;
}
</style>