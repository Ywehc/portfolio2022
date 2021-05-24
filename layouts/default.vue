<template>
  <div class="wrapper">
    <Nuxt class="main"/>
    <Nav class="menu"/>
    <Footer class="icons"/>
  </div>
</template>

<style lang="scss">
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
.wrapper {
  margin: auto;
}
.main {
  height: 540px;
}
.main, .menu {
  // controls how centered the main view appears
  margin-left: 24%;
}
</style>
