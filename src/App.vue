<template>
  <div id="app" ref="appRef">
    <FilterContrast />
    <FilterFire />
    <FilterFuse />
    <FilterFuseFont />
    <BehavirorLiHover />
  </div>
</template>

<script>
import FilterContrast from './components/filter/contrast';
import FilterFire from './components/filter/fire';
import FilterFuse from './components/filter/fuse';
import FilterFuseFont from './components/filter/fuse-font';
import BehavirorLiHover from './components/behaviror/li-hover';

export default {
  name: 'App',
  components: {
    FilterContrast,
    FilterFire,
    FilterFuse,
    FilterFuseFont,
    BehavirorLiHover
  },
  mounted() {
    console.log(this.$refs.appRef)
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
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
</style>
