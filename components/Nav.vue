<template>
    <div class="container">
        <div class="row">
            <div class="col-1 curve-container">
                <div class="curve"></div>
            </div>
            <div class="col-11 nav-container">
                <div class="nav-pane indigo"><NuxtLink to="/">Home</NuxtLink></div>
                <div class="nav-pane blue"><NuxtLink to="/about">About</NuxtLink></div>
                <div class="nav-pane green"><NuxtLink to="/skills">Skills</NuxtLink></div>
                <div class="nav-pane yellow"><NuxtLink to="/portfolio">Portfolio</NuxtLink></div>
                <div class="nav-pane orange"><NuxtLink to="/contact">Contact</NuxtLink></div>
            </div>
        </div>
        
    </div>
</template>

<style lang="scss" scoped>
@import '@/assets/scss/_global.scss';
.curve-container {
    position: relative;
    .curve {
        position: absolute;
        background: white;
        z-index: 2;
        height: 100em;
        width: 100em;
        border-radius: 50%;
        margin-top: -82em;
        margin-left: -44em;
    }
}
.nav-container {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
}
.nav-pane {
    height: $paneHeight;
    text-align: right;
    margin: $paneMargin;
    padding-top: 20px;
    a {
        color: black;
        font-size: 20px;
        font-weight: bold;
        background: white;
        padding: 10px;
        border-top-left-radius: 15%;
    }
}
.indigo {
    background-image: url('~/assets/images/indigo.png');
    background-size: cover;
    width: 60%;
}
.blue {
    background-image: url('~/assets/images/blue.png');
    background-size: cover;
    background-position-y: 95%;
    width: 70%;
}
.green {
    background-image: url('~/assets/images/green.png');
    background-size: cover;
    width: 80%;
}
.yellow {
    background-image: url('~/assets/images/yellow.png');
    background-size: cover;
    width: 90%;
}
.orange {
    background-image: url('~/assets/images/orange.png');
    background-size: 100%;
    width: 100%;
}
.corner {
  width: 160px;
    height: 0px;
    border-bottom: 40px solid red;
    border-right: 40px solid white;
}
</style>