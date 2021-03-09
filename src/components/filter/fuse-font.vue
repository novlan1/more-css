<template>
  <div class="container single-container">
    <!-- <h1>Blur word Animation</h1> -->
    <h1>Yang Guo Wang</h1>
  </div>
</template>
<script>
export default {
  
}
</script>
<style scoped lang="scss">
@import url(https://fonts.googleapis.com/css?family=Righteous);

// * {
//   box-sizing: border-box;
// }

// html,
// body {
//   height: 100%;
//   width: 100%;
//   background-color: black;
// }

.container {
  width: 100%;
  height: 100%;
  position: relative;
  padding: 2em;
  filter: contrast(20);
  background-color: black;
  overflow: hidden;
}

h1 {
  font-family: Righteous;
  color: white;
  font-size: 4rem;
  text-transform: uppercase;
  line-height: 1;
  animation: letterspacing 5s infinite alternate ease-in-out;
  display: block;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate3d(-50%, -50%, 0);
  letter-spacing: -2.2rem;
}

@keyframes letterspacing {
  0% {
    letter-spacing: -2.2rem;
    filter: blur(0.3rem);
  }

  50% {
    filter: blur(0.5rem);
  }

  100% {
    letter-spacing: 0.5rem;
    filter: blur(0rem);
    color: #fff;
  }
}
</style>