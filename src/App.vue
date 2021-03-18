<template>
  <div id="app">
    <FilterContrast />
    <FilterFire />
    <FilterFuse />
    <FilterFuseFont />
    <BehavirorLiHover />
    <MixBlend />
    <MixBlendWord />
    <ColorSelection />
    <ColorSignal />
    <FilterBlur />
    <InvertHueRotate />
    <FilterGrayScale />
    <BoxReflect />
    <FigureLineGradientBg />
    <FigureLineGradientWord />
    <FigureLineGradientShineWord />
    <FigureLineGradientCurve />
    <FigureBoxShadowFocus />
    <FigureBoxShadowSingleShadow />
    <FigureClipPath />
    <FigureClipSnake />
    <FigureConicGradientPieChart />
    <FigureConicGradientColorTable />
    <FigureConicGradientWallpaper />
    <FigureConicGradientRepeating />
    <FigureConicGradientAnima />
    <FigureLinearGradientSquareCell />
    <FigureLinearGradientRibbon />
    <FigureLinearGradientGrid />
    <FigureHeart />
    <!-- <FigureMask /> -->
    <CompIosSwitch />
    <CompTabNav />
    <MaskAngle />
    <MaskPics />
    <MaskAnima />
    <MaskMagicAnima />
    <MaskMagicTransition />
    <FigureBoxShadowCurve />
    <ColorBgBlendMode />
    <ColorBeautifulWord />
  </div>
</template>

<script>
import FilterContrast from './components/filter/contrast';
import FilterFire from './components/filter/fire';
import FilterFuse from './components/filter/fuse';
import FilterFuseFont from './components/filter/fuse-font';
import BehavirorLiHover from './components/behaviror/li-hover';
import MixBlend from './components/mix/mix-blend.vue';
import MixBlendWord from './components/mix/mix-blend-word.vue';
import ColorSelection from './components/color/selection';
import ColorSignal from './components/color/color-signal';
import FilterBlur from './components/filter/blur';
import InvertHueRotate from './components/filter/invert-hue-rotate';
import FilterGrayScale from './components/filter/grayscale';
import BoxReflect from './components/figure/box-reflect.vue';
import FigureLineGradientWord from './components/figure/linear-gradient-word';
import FigureLineGradientShineWord from './components/figure/linear-gradient-shine-word';
import FigureLineGradientCurve from './components/figure/linear-gradient-curve';
import FigureLineGradientBg from './components/figure/linear-gradient-bg';
import FigureBoxShadowFocus from './components/figure/box-shadow-focus';
import FigureBoxShadowSingleShadow from './components/figure/box-shadow-single-shadow';
import FigureClipPath from './components/figure/clip-path';
import FigureClipSnake from './components/figure/clip-snake';
import FigureConicGradientPieChart from './components/figure/conic-gradient-pie-chart';
import FigureConicGradientColorTable from './components/figure/conic-gradient-color-table';
import FigureConicGradientWallpaper from './components/figure/conic-gradient-wallpaper';
import FigureConicGradientRepeating from './components/figure/conic-gradient-repeating';
import FigureConicGradientAnima from './components/figure/conic-gradient-anima';
import FigureLinearGradientSquareCell from './components/figure/linear-gradient-square-cell'
import FigureLinearGradientRibbon from './components/figure/linear-gradient-ribbon';
import FigureLinearGradientGrid from './components/figure/linear-gradient-grid';
import FigureHeart from './components/figure/transform-heart';
import CompIosSwitch from './components/component/ios-switch'
import CompTabNav from './components/component/tab-nav';
import MaskAngle from './components/behaviror/mask-angle';
import MaskPics from './components/behaviror/mask-pics';
import MaskAnima from './components/behaviror/mask-anima';
import MaskMagicAnima from './components/behaviror/mask-magic-anima';
import MaskMagicTransition from './components/behaviror/mask-magic-transition';
import FigureBoxShadowCurve from './components/figure/box-shadow-curve';
import ColorBgBlendMode from './components/color/background-blend-mode';
import ColorBeautifulWord from './components/color/beautiful-word';
// import FigureMask from './components/figure/mask';

export default {
  name: 'App',
  components: {
    FilterContrast,
    FilterFire,
    FilterFuse,
    FilterFuseFont,
    BehavirorLiHover,
    MixBlend,
    MixBlendWord,
    ColorSelection,
    ColorSignal,
    FilterBlur,
    InvertHueRotate,
    FilterGrayScale,
    BoxReflect,
    FigureLineGradientWord,
    FigureLineGradientBg,
    FigureLineGradientCurve,
    FigureLineGradientShineWord,
    FigureBoxShadowFocus,
    FigureBoxShadowSingleShadow,
    FigureClipPath,
    FigureClipSnake,
    FigureConicGradientPieChart,
    FigureConicGradientColorTable,
    FigureConicGradientWallpaper,
    FigureConicGradientRepeating,
    FigureConicGradientAnima,
    FigureLinearGradientSquareCell,
    FigureLinearGradientRibbon,
    FigureLinearGradientGrid,
    FigureHeart,
    CompIosSwitch,
    CompTabNav,
    // FigureMask,
    MaskAngle,
    MaskPics,
    MaskAnima,
    MaskMagicAnima,
    MaskMagicTransition,
    FigureBoxShadowCurve,
    ColorBgBlendMode,
    ColorBeautifulWord,
  },
  mounted() {
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
button,
input,
select,
textarea {
  box-sizing: border-box;
  outline: none;
}
body {
  font-size: 14px;
}
ul,
li {
  list-style: none;
}
.single-container {
  overflow: hidden;
  position: relative;
  padding: 50px 0;
  border-bottom: 1px solid #ccc;
  min-height: 300px;
}
.single-container:before {
  left: 50%;
  top: 0;
  padding: 0 10px;
  border-radius: 0 0 5px 5px;
  max-width: 300px;
  line-height: 20px;
  content: attr(data-title);
  -webkit-transform: translateX(-50%);
  transform: translateX(-50%);

  position: absolute;
  z-index: 99999;
  color: #fff;

  background-color: #66f;
}
.flex-ct-x {
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  -webkit-justify-content: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-align-items: center;
  -ms-flex-align: center;
  align-items: center;
}
</style>
