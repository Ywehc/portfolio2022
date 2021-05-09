<template>
    <div class="container">
        <div class="row">
            <div class="col-1 curve-container">
                <div class="curve"></div>
            </div>
            <div class="col-11 nav-container">
                <div class="nav-pane indigo">
                        <NuxtLink class="link" to="/">Home</NuxtLink>
                </div>
                <div class="nav-pane blue">
                        <NuxtLink class="link" to="/about">About</NuxtLink>
                </div>
                <div class="nav-pane green">
                        <NuxtLink class="link" to="/skills">Skills</NuxtLink>
                </div>
                <div class="nav-pane yellow">
                        <NuxtLink class="link" to="/portfolio">Portfolio</NuxtLink>
                </div>
                <div class="nav-pane orange">
                        <NuxtLink class="link" to="/contact">Contact</NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '@/assets/scss/_global.scss';
@import '@/assets/scss/_nav.scss';

</style>