<template>
    <div class="container">
        <div class="row mt-xl-auto">
            <div class="col left d-none d-lg-block">
              <IndexAnimation class="animation d-none d-lg-block"/>
            </div>
            <div class="col d-flex right">
              <h1 class="title">Chris Kieran</h1>
              <h2 class="subtitle">Frontend Web Developer</h2>
              <p class="d-xl-none">"Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?"</p>
              <p class="d-xl-none">"Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?"</p>
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
}
h2 {
  font-size: 24px;
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
  .right {
    align-items: center;
  }
}
</style>