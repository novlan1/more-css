<template>
  <div class="container single-container" data-title="火焰效果">
    <div class="g-container">
      <div class="g-fire">
        <div 
          v-for="(item, index) of new Array(40)" 
          :key="index"
          class="g-dot"
        >
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style>
:root {
  --fireWidth: 115px;
  --fireHeight: 200px;
  --dotSize: 24px;
  --fireColor: #b5932f;
  --fireColor: #008eff;
  --fireColor: #ff9900;
}
</style>
<style lang="scss" scoped>
$douCount: 40;
$animationTime: 2;
$delayTime: 3;

@function randomNum($max, $min: 0) {
  @return ($min + random($max));
}

.container {
  background: #000;
  overflow: hidden;
}

.g-container {
  position: relative;
  width: 384px;
  height: 300px;
  margin: 0 auto;
  background-color: #000;
}

.g-fire {
  position: absolute;
  width: 0;
  height: 0;
  bottom: 100px;
  left: 50%;
  border-radius: 45%;
  box-sizing: border-box;
  border: 200px solid #000;
  border-bottom: 200px solid transparent;
  transform: translate(-50%, 0) scaleX(0.4);
  background-color: var(--fireColor);
  filter: blur(20px) contrast(30);
}

.g-dot {
  position: absolute;
  bottom: -210px;
  left: 0;
  width: var(--dotSize);
  height: var(--dotSize);
  background: #000;
  border-radius: 50%;
}

@for $i from 1 to $douCount + 1 {
  .g-dot:nth-child(#{$i}) {
    bottom: -#{randomNum(120, 240)}px;
    left: #{randomNum(300, -160)}px;
    animation: move
      #{randomNum($animationTime * 13, 7) /
      10}s
      infinite
      #{randomNum($delayTime * 20) /
      10}s
      linear;
  }
}

@keyframes move {
  100% {
    transform: translate3d(0, -350px, 0);
  }
}
</style>