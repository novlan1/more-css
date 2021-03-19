<template>
	<div class="single-container flex-ct-x" data-title="抖动动画">
    <img class="img" src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBzdGFuZGFsb25lPSJubyI/PjwhRE9DVFlQRSBzdmcgUFVCTElDICItLy9XM0MvL0RURCBTVkcgMS4xLy9FTiIgImh0dHA6Ly93d3cudzMub3JnL0dyYXBoaWNzL1NWRy8xLjEvRFREL3N2ZzExLmR0ZCI+PHN2ZyB0PSIxNTYwNjE5NDI3MzQwIiBjbGFzcz0iaWNvbiIgc3R5bGU9IiIgdmlld0JveD0iMCAwIDEwMjQgMTAyNCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHAtaWQ9IjEyODUwIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgd2lkdGg9IjIwMCIgaGVpZ2h0PSIyMDAiPjxkZWZzPjxzdHlsZSB0eXBlPSJ0ZXh0L2NzcyI+PC9zdHlsZT48L2RlZnM+PHBhdGggZD0iTTUzNi44MTY5NDEgMzA0LjY3MDExOEM0OTUuNjgxMDEyIDMwNC42NTI1NjMgNDU0LjkxMTIxOSAzMTIuMzk3ODAyIDQxNi42NDc1MjkgMzI3LjQ5OTI5NEw0MTYuNjQ3NTI5IDM5LjE1Mjk0MSAxOTcuNTExNTI5IDYuOTI3MDU5IDE4OS43NDExNzYgMTAyLjQgMTc0LjY4MjM1MyAzLjU1Mzg4MiAxNTAuNTg4MjM1IDAgMjI1Ljg4MjM1MyAxMDE5Ljk2NDIzNSA0MTYuNjQ3NTI5IDk3OC44MjM1MjkgNDE2LjY0NzUyOSA5NTEuNzE3NjQ3QzQ1NC45MDk2MDQgOTY2LjgyNDcxMyA0OTUuNjgwNDcgOTc0LjU3MDE1MyA1MzYuODE2OTQxIDk3NC41NDY4MjQgNzE5LjY5MTI5NCA5NzQuNTQ2ODI0IDg2OC4xMTEwNTkgODI0LjY4MTQxMiA4NjguMTExMDU5IDYzOS43NTkwNTkgODY4LjExMTA1OSA0NTQuODM2NzA2IDcxOS42MzEwNTkgMzA0LjY3MDExOCA1MzYuODE2OTQxIDMwNC42NzAxMThNNDM2LjU4NTQxMiA2MjguNzk2MjM1QzQzNy41MTM3MTUgNTY2LjU0MDkxNSA0ODguNTc1OTUxIDUxNi43MzkwNzMgNTUwLjgzNTAyOCA1MTcuMzY2Njk4IDYxMy4wOTQxMDYgNTE3Ljk5NDMyNCA2NjMuMTQxOTc2IDU2OC44MTU0NDMgNjYyLjgxNTA0MyA2MzEuMDc2ODI4IDY2Mi40ODgxMSA2OTMuMzM4MjA4IDYxMS45MDkyOTQgNzQzLjYzMDkzOCA1NDkuNjQ3MDU5IDc0My42MDQ3MDYgNDg2LjcyODY5OSA3NDMuMTA3NjAyIDQzNi4xMTc4NjQgNjkxLjcxNDgxOSA0MzYuNTg1NDEyIDYyOC43OTYyMzVNNjgyLjE2NDcwNiA3NTEuOTE3MTc2QzYwNy43NzQxMTggODE2LjY3MDExOCA1MzMuMDgyMzUzIDc3OS4wMjMwNTkgNTMzLjA4MjM1MyA3NzkuMDIzMDU5IDUzMy4wODIzNTMgNzc5LjAyMzA1OSA1ODUuNzg4MjM1IDgwMy4xMTcxNzYgNjYxLjA4MjM1MyA3MzkuODcwMTE4IDczNi4zNzY0NzEgNjc2LjYyMzA1OSA2ODkuNjk0MTE4IDU2OC4xOTk1MjkgNjg5LjY5NDExOCA1NjguMTk5NTI5IDY4OS42OTQxMTggNTY4LjE5OTUyOSA3NjMuNDgyMzUzIDY4MS4xNDA3MDYgNjgyLjE2NDcwNiA3NTEuOTE3MTc2IiBwLWlkPSIxMjg1MSIgZmlsbD0iI2ZmNjY2NiI+PC9wYXRoPjwvc3ZnPg==">
	</div>
</template>
<style scoped lang='scss'>
.img {
  display: inline-block;
  height: 10vmin;
  vertical-align: super;
  -webkit-animation: swing 3s infinite;
  animation: swing 3s infinite;
}
@keyframes swing {
  0%,
  65% {
    -webkit-transform: rotate(0);
    transform: rotate(0);
  }

  70% {
    -webkit-transform: rotate(6deg);
    transform: rotate(6deg);
  }
  75% {
    -webkit-transform: rotate(-6deg);
    transform: rotate(-6deg);
  }
  80% {
    -webkit-transform: rotate(6deg);
    transform: rotate(6deg);
  }
  85% {
    -webkit-transform: rotate(-6deg);
    transform: rotate(-6deg);
  }
  90% {
    -webkit-transform: rotate(6deg);
    transform: rotate(6deg);
  }
  95% {
    -webkit-transform: rotate(-6deg);
    transform: rotate(-6deg);
  }
  100% {
    -webkit-transform: rotate(0);
    transform: rotate(0);
  }
}
</style>