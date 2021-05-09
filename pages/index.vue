<template>
    <div class="container">
        <div class="row mt-auto">
            <div class="col left">
              <IndexAnimation />
            </div>
            <div class="col d-flex right">
              <h1 class="title">Chris Kieran</h1>
              <h2 class="subtitle">Frontend Web Developer</h2>
              <div class="nav-pane red"></div>
              <div class="nav-pane violet"></div>
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
}
h2 {
  font-size: 26px;
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
.red {
    background-image: url('~/assets/images/red.png');
    background-size: cover;
    background-position-y: 75%;
    width: 75%;
}
.violet {
    background-image: url('~/assets/images/violet.png');
    background-size: cover;
    background-position-y: 75%;
    width: 100%;
}
.left {
  border: 2px solid blue;
  margin-left: 90px;
  margin-top: -120px;
}

</style>