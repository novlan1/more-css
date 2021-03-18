<template>
	<div class="single-container flex-ct-x" data-title="使用box-shadow绘制曲线">
		<div class="line"></div>
    <div class="reverseline"></div>
    <div class="colorline"></div>
    <div class="middle"></div>
	</div>
</template>
<style scoped lang='scss'>
@function fact($number) {
  $value: 1;
  @if $number>0 {
    @for $i from 1 through $number {
      $value: $value * $i;
    }
  }
  @return $value;
}

@function pow($number, $exp) {
  $value: 1;
  @if $exp>0 {
    @for $i from 1 through $exp {
      $value: $value * $number;
    }
  } @else if $exp < 0 {
    @for $i from 1 through -$exp {
      $value: $value / $number;
    }
  }
  @return $value;
}

@function rad($angle) {
  $unit: unit($angle);
  $unitless: $angle / ($angle * 0 + 1);
  @if $unit==deg {
    $unitless: $unitless / 180 * pi();
  }
  @return $unitless;
}

@function pi() {
  @return 3.14159265359;
}

@function sin($angle) {
  $sin: 0;
  $angle: rad($angle);
  // Iterate a bunch of times.
  @for $i from 0 through 15 {
    $sin: $sin + pow(-1, $i) * pow($angle, (2 * $i + 1)) / fact(2 * $i + 1);
  }
  @return $sin;
}

@function cos($angle) {
  $cos: 0;
  $angle: rad($angle);
  // Iterate a bunch of times.
  @for $i from 0 through 15 {
    $cos: $cos + pow(-1, $i) * pow($angle, 2 * $i) / fact(2 * $i);
  }
  @return $cos;
}

@function tan($angle) {
  @return sin($angle) / cos($angle);
}

@function shadowSet($vx, $vy, $direction, $count, $color) {
  $shadow: 0 0 0 0 $color;

  @for $i from 0 through $count {
    $x: sin($i / 8) * $vx * $direction;
    $y: $i * $vy;

    $shadow: $shadow, #{$x} #{$y} 0 0 $color;
  }

  @return $shadow;
}

@function shadowSetColor($vx, $vy, $direction, $count, $color) {
  $shadow: 0 0 0 0 $color;

  @for $i from 0 through $count {
    $color: lighten($color, 0.5);

    $x: sin($i / 8) * $vx * $direction;
    $y: $i * $vy;

    $shadow: $shadow, #{$x} #{$y} 0 0 $color;
  }

  @return $shadow;
}

.single-container {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.middle {
  width: 20px;
  height: 20px;
  background: #000;
  margin: 10vh auto;
  border-radius: 50%;
  box-shadow: shadowSet(5vmin, 1.4vmin, 1, 50, #000);
}

.line {
  width: 1px;
  height: 1px;
  margin: 10vh auto;
  background: #000;
  border-radius: 50%;
  box-shadow: shadowSet(4px, 1px, 1, 50, #000);
}

.reverseline {
  width: 1px;
  height: 1px;
  margin: 10vh auto;
  background: #000;
  border-radius: 50%;
  box-shadow: shadowSet(8px, 2px, -1, 100, red);
}

.colorline {
  width: 5px;
  height: 5px;
  margin: 10vh auto;
  background: green;
  border-radius: 50%;
  box-shadow: shadowSetColor(8px, 2px, -1, 100, green);
}
</style>