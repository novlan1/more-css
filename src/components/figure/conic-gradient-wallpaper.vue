<template>
	<div class="single-container flex-ct-x" data-title="使用conic-gradient()描绘锥形墙纸">
    <div class="basis"></div>
    <div class="wallpaper"></div>
    <div class="wallpaper2"></div>
	</div>
</template>

<style lang="scss" scoped>
.basis {
  width: 250px;
  height: 250px;
  margin: 50px auto;
  background: conic-gradient(
    #000 12.5%,
    #fff 0 37.5%,
    #000 0 62.5%,
    #fff 0 87.5%,
    #000 0
  );
  border: 5px solid #999;
}

.wallpaper {
  width: 250px;
  height: 250px;
  margin: 50px auto;
  background: conic-gradient(
    #000 12.5%,
    #fff 0 37.5%,
    #000 0 62.5%,
    #fff 0 87.5%,
    #000 0
  );
  background-size: 50px 50px;
  border: 5px solid #999;
}

.wallpaper2 {
  width: 250px;
  height: 250px;
  margin: 50px auto;
  background: conic-gradient(
    #000 12.5%,
    #fff 0 37.5%,
    #000 0 62.5%,
    #fff 0 87.5%,
    #000 0
  );
  background-size: 50px 50px;
  border-radius: 50%;
  border: 5px solid #999;
}
</style>