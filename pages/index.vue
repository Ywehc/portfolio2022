<template>
    <div class="container">
        <div class="row mt-xl-auto">
            <div class="col left d-none d-xl-block">
              <RecursiveTree class="animation"/>
            </div>
            <div class="col d-flex right">
              <div class="mobile-animation">
                  <h1 class="title">Chris Kieran</h1>
                  <h2 class="subtitle">Frontend Developer</h2>
              </div>
              <div class="nav-pane pane-7 d-none d-xl-block"></div>
              <div class="nav-pane pane-6 d-none d-xl-block"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
@import '~/assets/scss/_global.scss';

.container {
  display: flex;
  padding-right: 0;
}
.row {
  width: 100%;
}
h1 {
  font-size: $headingFontSize;
  margin-bottom: 0;
  text-align: right;
}
h2 {
  font-size: 29px;
  text-align: right;
}
h1, h2 {
  font-family: 'Questrial', sans-serif;
}
.title, .subtitle {
  z-index: 3;
}
.nav-pane {
    height: $paneHeight;
    margin: $paneMargin;
}
.right {
    flex-direction: column;
    align-items: flex-end;
    padding-right: 0;
}
.pane-7 {
    background-image: url('~/assets/images/violet.png');
    background-size: cover;
    width: 77%;
    background-position-y: 70%;
}
.pane-6 {
    background-image: url('~/assets/images/red.png');
    background-size: cover;
    width: 100%;
    background-position-y: -5px;
}
.left {
  margin-left: 110px;
  margin-top: -120px;
}
.animation {
  right: 160px;
}
@media screen and (max-width: 1200px) {
  h1 {
    text-align: center;
    font-size: 34px;
  }
  h2 {
    font-size: 20px;
    margin-bottom: 0;
  }
  .right {
    align-items: center;
    height: 60vh;
    overflow: hidden;
  }
  .quote-container {
    padding-top: 18em;
    p {
      font-size: 14px;
    }
  }
  // animated backglow inspired by George Hastings https://codepen.io/georgehastings/pen/xgwxgo

  @mixin backlight($x, $y, $spread, $size, $colorA, $colorB, $duration) {
    &:after {
      position: absolute;
      content: "";
      top: $y;
      left: $x;
      right: 0;
      z-index: -1;
      height: 100%;
      width: 100%;
      margin: 0 auto;
      transform: scale($size);
      -webkit-filter: blur($spread);
      -moz-filter: blur($spread);
      -ms-filter: blur($spread);
      filter: blur($spread);
      background: linear-gradient(270deg, $colorA, $colorB);
      background-size: 200% 200%;
      animation: animateGlow $duration ease infinite;
      
      @keyframes animateGlow {
        0%{background-position:0% 50%}
        50%{background-position:100% 50%}
        100%{background-position:0% 50%}
      }
    }
  }
  .mobile-animation {
    margin-top: 20vh;
    position: relative;
    height: 20vw;
    line-height: 30vw;
    text-align: center;
    color: #252B37;
    // background-color: #151823;
    background-color: black;
    animation: textColor 10s ease infinite;
    @include backlight(0, 5vw, 5vw, 0.75, #0fffc1, #7e0fff, 10s);
      
    @keyframes textColor {
      0% {
        color: #7e0fff;
      }
      50% {
        color: #0fffc1;
      }
      100% {
        color: #7e0fff;
      }
    }
  }
}
</style>