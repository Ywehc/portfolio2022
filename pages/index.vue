<template>
    <div class="container">
        <div class="row mt-auto">
            <div class="col left">
              <IndexAnimation class="animation"/>
            </div>
            <div class="col d-flex right">
              <h1 class="title">Chris Kieran</h1>
              <h2 class="subtitle">Frontend Web Developer</h2>
              <div class="nav-pane pane-7"></div>
              <div class="nav-pane pane-6"></div>
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
  font-size: 52px;
  margin-bottom: 0;
}
h2 {
  font-size: 28px;
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
  right: 120px;
}

</style>