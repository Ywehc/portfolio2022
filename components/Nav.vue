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
@import '@/assets/scss/_nav.scss';

</style>