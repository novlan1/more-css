<template>
  <div class="single-container">
    <div class="container">
      <div v-for="(item, index) of new Array(6)" :key="index" class="box">
      </div>
    </div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style scoped lang="scss">
$count: 6;
$each: 360deg / $count;
$distance: 100px;
$boxshadow: 25px;

.single-container {
  background-color: #000;
  overflow: hidden;
}

.container {
  position: absolute;
  width: 200px;
  height: 200px;
  transform: translate(-50%, -50%);
  top: 50%;
  left: 50%;
}

.box {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  border: 1px solid #fff;
  background: rgb(0, 0, 0);
  box-shadow: inset 0 $boxshadow 0 $boxshadow rgb(255, 255, 255);
  mix-blend-mode: difference;
}

@for $i from 1 through $count {
  $curRotate: $i * $each;

  .box:nth-child(#{$i}) {
    transform: rotate($curRotate) translate(0, 50%);
    animation: move#{$i} 10s linear infinite alternate;
  }

  @keyframes move#{$i} {
    100% {
      transform: rotate(calc(1080deg + #{$curRotate})) translate($distance);
    }
  }
}

@for $i from 1 through $count {
}
</style>