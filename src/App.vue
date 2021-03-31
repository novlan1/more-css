<template>
  <div id="app">
    <FilterContrast />
    <FilterFire />
    <FilterFuse />
    <FilterFuseFont />
    <BehaviorLiHover />
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
    <LinearGraStripeText />
    
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
    <FigureAnimaSwing />
    <LayoutClipPath />
    <LayoutFloatAround />
    <LayoutReverseText />
    <LayoutTransReverseText />
    <LayoutTransHalfPx />
    <LayoutWritingMode />
    <div class="behavior">
      <BehaviorEmptyState />
      <BehaviorFocusWithin />
      <BehaviorHoverTips />
      <BehaviorDynamicBorder />
      <BehaviorMouseFollowing />
      <BehaviorClearAttr />
      <BehaviorClearChild />
      <BehaviorFormValid />
      <BehaviorBeautiSelection />
      <BehaviorAnimationDealy />
      <BehaviorAutoHeight />
      <BehaviorObjectFit />
      <BehaviorPositionSticky />
      <BehaviorTextAlignLast />
      <BehaviorBoxShadowRainbow />
    </div>
  </div>
</template>

<script>
import FilterContrast from './components/filter/contrast';
import FilterFire from './components/filter/fire';
import FilterFuse from './components/filter/fuse';
import FilterFuseFont from './components/filter/fuse-font';
import BehaviorLiHover from './components/behavior/li-hover';
import MixBlend from './components/mix/mix-blend.vue';
import MixBlendWord from './components/mix/mix-blend-word.vue';
import ColorSelection from './components/color/selection';
import ColorSignal from './components/color/colorful-signal-bar';
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
import MaskAngle from './components/behavior/mask-angle';
import MaskPics from './components/behavior/mask-pics';
import MaskAnima from './components/behavior/mask-anima';
import MaskMagicAnima from './components/behavior/mask-magic-anima';
import MaskMagicTransition from './components/behavior/mask-magic-transition';
import FigureBoxShadowCurve from './components/figure/box-shadow-curve';
import ColorBgBlendMode from './components/color/background-blend-mode';
import ColorBeautifulWord from './components/color/beautiful-word';
import FigureAnimaSwing from './components/figure/animation-swing';

import LayoutClipPath from './components/layout/cilp-path';
import LayoutFloatAround from './components/layout/float-around';
import LayoutReverseText from './components/layout/letter-spacing-reverse-text';
import LayoutTransReverseText from './components/layout/transform-reverse-text';
import LayoutTransHalfPx from './components/layout/transform-half-px';
import LayoutWritingMode from './components/layout/writing-mode';

import BehaviorEmptyState from './components/behavior/empty-state';
import BehaviorFocusWithin from './components/behavior/focus-within';
import BehaviorHoverTips from './components/behavior/hover-tips';
import BehaviorDynamicBorder from './components/behavior/dynamic-border';
import BehaviorMouseFollowing from './components/behavior/mouse-following';
import BehaviorClearAttr from './components/behavior/clear-attr';
import BehaviorClearChild from './components/behavior/nth-child';
import BehaviorFormValid from './components/behavior/form-valid';
import BehaviorBeautiSelection from './components/behavior/beauti-selection';
import BehaviorAnimationDealy from './components/behavior/animation-delay';
import BehaviorAutoHeight from './components/behavior/auto-height';
import BehaviorObjectFit from './components/behavior/object-fit';
import BehaviorPositionSticky from './components/behavior/position-sticky';
import BehaviorTextAlignLast from './components/behavior/text-align-last';
import BehaviorBoxShadowRainbow from './components/color/box-shadow-rainbow';
import LinearGraStripeText from './components/figure/linear-gradient-stripe-text'
// import FigureMask from './components/figure/mask';

export default {
  name: 'App',
  components: {
    FilterContrast,
    FilterFire,
    FilterFuse,
    FilterFuseFont,
    BehaviorLiHover,
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
    FigureAnimaSwing,
    LayoutClipPath,
    LayoutFloatAround,
    LayoutReverseText,
    LayoutTransReverseText,
    LayoutTransHalfPx,
    LayoutWritingMode,
    BehaviorEmptyState,
    BehaviorFocusWithin,
    BehaviorHoverTips,
    BehaviorDynamicBorder,
    BehaviorMouseFollowing,
    BehaviorClearAttr,
    BehaviorClearChild,
    BehaviorFormValid,
    BehaviorBeautiSelection,
    BehaviorAnimationDealy,
    BehaviorAutoHeight,
    BehaviorObjectFit,
    BehaviorPositionSticky,
    BehaviorTextAlignLast,
    BehaviorBoxShadowRainbow,
    LinearGraStripeText,
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

  background-color: #66f;
}

.single-container:after {
  right: 0;
  bottom: 0;
  padding: 5px 10px;
  border-top-left-radius: 5px;
  background-color: #ccc;
  font-weight: 700;
  font-size: 16px;
}
.behavior .single-container:after {
  content: "行为";
}

.single-container:after,
.single-container:before {
  position: absolute;
  z-index: 99999;
  color: #fff;
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
