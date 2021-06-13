<template>
  <div class="wrapper">
    <Nuxt class="main"/>
    <Nav class="menu"/>
    <Footer class="d-none d-xl-flex"/>
  </div>
</template>

<style lang="scss">
html {
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
  height: 460px;
  padding-right: 9em!important;
}
.menu {
  padding-right: 10em;
}

@media screen and (max-width: 1200px) {
  .wrapper {
    background-color: black;
    height: 100vh;
  }
  .main {
    min-height: 80vh;
    text-align: center;
    padding-right: 15px!important;
    color: white;
    overflow: scroll;
  }
  .menu {
    padding-right: 15px;
    .nav-container {
      background: black!important;
      color: white;
    }
  }
}
</style>
