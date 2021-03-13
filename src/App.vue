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
    FigureClipSnake
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
