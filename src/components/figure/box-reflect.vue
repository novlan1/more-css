<template>
  <div class="single-container" data-title="使用box-reflex制作艺术图案">
    <div class="g-wrap1">
    <div class="g-wrap2">
        <div class="g-wrap3">
            <div class="g-wrap4"></div>
            </div>
        </div>
    </div>

    <div class="g-wrap1 radial">
        <div class="g-wrap2">
            <div class="g-wrap3">
                <div class="g-wrap4"></div>
            </div>
        </div>
    </div>

    <div class="g-wrap1 negative">
        <div class="g-wrap2">
            <div class="g-wrap3">
                <div class="g-wrap4"></div>
            </div>
        </div>
    </div>

    <div class="g-wrap1 line">
        <div class="g-wrap2">
            <div class="g-wrap3">
                <div class="g-wrap4"></div>
            </div>
        </div>
    </div>

    <div class="g-wrap1 line2">
        <div class="g-wrap2">
            <div class="g-wrap3">
                <div class="g-wrap4"></div>
            </div>
        </div>
    </div>

    <div class="g-wrap1 line3">
        <div class="g-wrap2">
            <div class="g-wrap3">
                <div class="g-wrap4"></div>
            </div>
        </div>
    </div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style scoped lang="scss">
.single-container {
  width: 100%;
  height: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
}

// .g-wrap1 {
//     margin: auto;
// }

.g-wrap4 {
  width: 50px;
  height: 50px;
  background: linear-gradient(
    45deg,
    #000 10%,
    transparent 10%,
    transparent 30%,
    #000 30%,
    #000 50%,
    transparent 50%,
    transparent 70%,
    #000 70%,
    #000 90%,
    transparent 0
  );
}

.radial {
  .g-wrap4 {
    width: 50px;
    height: 50px;
    background: radial-gradient(
        circle at 0 0,
        #000 30%,
        transparent 30%,
        transparent 40%,
        #000 40%,
        #000 50%,
        transparent 50%
      ),
      radial-gradient(
        circle at 100% 100%,
        #000 10%,
        transparent 10%,
        transparent 30%,
        #000 30%,
        #000 40%,
        transparent 40%
      );
  }
}

.g-wrap4 {
  -webkit-box-reflect: right 0px;
}
.g-wrap3 {
  -webkit-box-reflect: below 0px;
}
.g-wrap2 {
  -webkit-box-reflect: left 0px;
}
.g-wrap1 {
  -webkit-box-reflect: above 0px;
}

.negative {
  .g-wrap4 {
    background: repeating-linear-gradient(
      45deg,
      #f7a37b,
      #f7a37b 10px,
      #ffdea8 10px,
      #ffdea8 20px,
      #d0e4b0 20px,
      #d0e4b0 30px,
      #7cc5d0 30px,
      #7cc5d0 40px,
      #00a2e1 40px,
      #00a2e1 50px,
      #0085c8 50px
    );
  }

  .g-wrap4 {
    -webkit-box-reflect: right 0px;
  }
  .g-wrap3 {
    -webkit-box-reflect: below 0px;
  }
  .g-wrap2 {
    -webkit-box-reflect: left 0px;
  }
  &.g-wrap1 {
    -webkit-box-reflect: above 0px;
  }
}

.line {
  .g-wrap4 {
    background: radial-gradient(
        circle at 150% 0,
        transparent 50%,
        #000 50%,
        #000 calc(50% + 2px),
        transparent calc(50% + 2px)
      ),
      radial-gradient(
        circle at 0 150%,
        transparent 50%,
        #000 50%,
        #000 calc(50% + 2px),
        transparent calc(50% + 2px)
      ),
      radial-gradient(
        circle at 50% 50%,
        transparent 50%,
        #000 50%,
        #000 calc(50% + 2px),
        transparent calc(50% + 2px)
      ),
      radial-gradient(
        circle at 20% 20%,
        transparent 20%,
        #000 20%,
        #000 calc(20% + 2px),
        transparent calc(20% + 2px)
      );
  }
}

.line2 {
  .g-wrap4 {
    background: radial-gradient(
        circle at 180% 0,
        transparent 70%,
        #000 70%,
        #000 calc(70% + 2px),
        transparent calc(70% + 2px)
      ),
      radial-gradient(
        circle at 0 180%,
        transparent 70%,
        #000 70%,
        #000 calc(70% + 2px),
        transparent calc(70% + 2px)
      ),
      radial-gradient(
        circle at 70% 70%,
        transparent 70%,
        #000 70%,
        #000 calc(70% + 2px),
        transparent calc(70% + 2px)
      ),
      radial-gradient(
        circle at 20% 20%,
        transparent 20%,
        #000 20%,
        #000 calc(20% + 2px),
        transparent calc(20% + 2px)
      ),
      radial-gradient(
        at 200% 200%,
        transparent 75%,
        #000 75%,
        #000 calc(75% + 2px),
        transparent calc(75% + 2px)
      );
  }
}

.line3 {
  .g-wrap4 {
    background: radial-gradient(
        circle at 70% 70%,
        transparent 30%,
        #000 30%,
        #000 calc(30% + 2px),
        transparent calc(30% + 2px)
      ),
      radial-gradient(
        circle at 0 120%,
        transparent 50%,
        #000 50%,
        #000 calc(50% + 2px),
        transparent calc(50% + 2px)
      ),
      radial-gradient(
        circle at 50% 70%,
        transparent 70%,
        #000 70%,
        #000 calc(70% + 2px),
        transparent calc(70% + 2px)
      ),
      radial-gradient(
        circle at 30% 20%,
        transparent 45%,
        #000 45%,
        #000 calc(45% + 2px),
        transparent calc(45% + 2px)
      ),
      radial-gradient(
        at -150% -150%,
        transparent 75%,
        #000 75%,
        #000 calc(75% + 2px),
        transparent calc(75% + 2px)
      ),
      conic-gradient(transparent 60%, #000 60%, #000 61%, transparent 61%);
  }
}

// @keyframes show {
//     0% {
//         opacity: 0;
//     }
//     100% {
//         opacity: 1;
//     }

// }
</style>