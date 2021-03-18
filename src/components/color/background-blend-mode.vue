<template>
	<div class="single-container flex-ct-x" data-title="使用background-blend-mode制作hover效果">
		<div class="pic"></div>
    <div class="pic pic1"></div>
    <div class="pic pic2"></div>
    <div class="pic pic3"></div>
	</div>
</template>

<style lang="scss" scoped>
$img: "https://user-images.githubusercontent.com/8554143/34238564-52f2ceb6-e63d-11e7-9812-dd987f98e9da.png";

.pic {
  width: 300px;
  height: 200px;
  margin: 30px;
  float: left;
  background: url($img), linear-gradient(#f00, #00f);
  background-size: cover, 100% 100%;
  background-position: 0 0, -300px 0;
  background-blend-mode: luminosity;
  background-repeat: no-repeat;
  transition: 0.5s background-position linear;
  cursor: pointer;
}

.pic1 {
  background-image: url($img), linear-gradient(90deg, #ff5722, #03a9f4);
}

.pic2 {
  background-image: url($img), linear-gradient(-180deg, #00bcd4, #fa1a09);
}

.pic3 {
  background-image: url($img),
    linear-gradient(45deg, #ffc107, #3f51b5, #4caf50, #ff0057, #fae105, #5c00ff);
}

.pic:hover {
  background-position: 0 0, 0 0;
}
</style>